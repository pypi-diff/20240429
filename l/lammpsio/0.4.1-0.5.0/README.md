# Comparing `tmp/lammpsio-0.4.1.tar.gz` & `tmp/lammpsio-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lammpsio-0.4.1.tar", last modified: Thu Jul 20 21:14:16 2023, max compression
+gzip compressed data, was "lammpsio-0.5.0.tar", last modified: Mon Apr 29 17:46:29 2024, max compression
```

## Comparing `lammpsio-0.4.1.tar` & `lammpsio-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:14:16.950640 lammpsio-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-20 21:14:05.000000 lammpsio-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-20 21:14:16.950640 lammpsio-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-20 21:14:05.000000 lammpsio-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-20 21:14:05.000000 lammpsio-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-20 21:14:16.950640 lammpsio-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:14:05.000000 lammpsio-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:14:16.950640 lammpsio-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:14:16.950640 lammpsio-0.4.1/src/lammpsio/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-20 21:14:05.000000 lammpsio-0.4.1/src/lammpsio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-20 21:14:05.000000 lammpsio-0.4.1/src/lammpsio/box.py
--rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-07-20 21:14:05.000000 lammpsio-0.4.1/src/lammpsio/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15907 2023-07-20 21:14:05.000000 lammpsio-0.4.1/src/lammpsio/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-07-20 21:14:05.000000 lammpsio-0.4.1/src/lammpsio/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:14:16.950640 lammpsio-0.4.1/src/lammpsio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-20 21:14:16.000000 lammpsio-0.4.1/src/lammpsio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-20 21:14:16.000000 lammpsio-0.4.1/src/lammpsio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:14:16.000000 lammpsio-0.4.1/src/lammpsio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 21:14:16.000000 lammpsio-0.4.1/src/lammpsio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 21:14:16.000000 lammpsio-0.4.1/src/lammpsio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:14:16.950640 lammpsio-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-20 21:14:05.000000 lammpsio-0.4.1/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-07-20 21:14:05.000000 lammpsio-0.4.1/tests/test_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-20 21:14:05.000000 lammpsio-0.4.1/tests/test_dump_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-20 21:14:05.000000 lammpsio-0.4.1/tests/test_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:29.794054 lammpsio-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-29 17:46:23.000000 lammpsio-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-04-29 17:46:29.794054 lammpsio-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-29 17:46:23.000000 lammpsio-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-29 17:46:23.000000 lammpsio-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-29 17:46:29.794054 lammpsio-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:46:23.000000 lammpsio-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:29.790054 lammpsio-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:29.794054 lammpsio-0.5.0/src/lammpsio/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-29 17:46:23.000000 lammpsio-0.5.0/src/lammpsio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-29 17:46:23.000000 lammpsio-0.5.0/src/lammpsio/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-04-29 17:46:23.000000 lammpsio-0.5.0/src/lammpsio/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-04-29 17:46:23.000000 lammpsio-0.5.0/src/lammpsio/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18363 2024-04-29 17:46:23.000000 lammpsio-0.5.0/src/lammpsio/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-29 17:46:23.000000 lammpsio-0.5.0/src/lammpsio/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:29.794054 lammpsio-0.5.0/src/lammpsio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-04-29 17:46:29.000000 lammpsio-0.5.0/src/lammpsio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-29 17:46:29.000000 lammpsio-0.5.0/src/lammpsio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:46:29.000000 lammpsio-0.5.0/src/lammpsio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 17:46:29.000000 lammpsio-0.5.0/src/lammpsio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 17:46:29.000000 lammpsio-0.5.0/src/lammpsio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:29.794054 lammpsio-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-29 17:46:23.000000 lammpsio-0.5.0/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-29 17:46:23.000000 lammpsio-0.5.0/tests/test_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-29 17:46:23.000000 lammpsio-0.5.0/tests/test_dump_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-04-29 17:46:23.000000 lammpsio-0.5.0/tests/test_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-29 17:46:23.000000 lammpsio-0.5.0/tests/test_topology.py
```

### Comparing `lammpsio-0.4.1/LICENSE` & `lammpsio-0.5.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021-2023, Auburn University
+Copyright (c) 2021-2024, Auburn University
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright
```

### Comparing `lammpsio-0.4.1/PKG-INFO` & `lammpsio-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammpsio
-Version: 0.4.1
+Version: 0.5.0
 Summary: Python tools for working with LAMMPS
 Home-page: https://github.com/mphowardlab/lammpsio
 Author: Michael P. Howard
 Author-email: mphoward@auburn.edu
 Project-URL: Source Code, https://github.com/mphowardlab/lammpsio
 Project-URL: Issue Tracker, https://github.com/mphowardlab/lammpsio/issues
 Classifier: Intended Audience :: Science/Research
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: packaging
 
 # lammpsio
 
 [![PyPI version](https://img.shields.io/pypi/v/lammpsio.svg)](https://pypi.org/project/lammpsio)
 [![PyPI downloads](https://img.shields.io/pypi/dm/lammpsio)](https://pypi.org/project/lammpsio)
 [![Conda](https://img.shields.io/conda/dn/conda-forge/lammpsio)](https://anaconda.org/conda-forge/lammpsio)
 
@@ -46,39 +48,69 @@
     snapshot = lammpsio.Snapshot(3, box, step=100)
 
 These constructor arguments are available as attributes:
 
 - `N`: number of particles (int)
 - `box`: bounding box (`Box`)
 - `step`: timestep counter (int)
+- `num_types`: number of particle types (int). If `num_types is None`, then the number of types is deduced from `typeid`.
 
 The data contained in a `Snapshot` per particle is:
 
 - `id`: (*N*,) array atom IDs (dtype: `int`, default: runs from 1 to *N*)
 - `position`: (*N*,3) array of coordinates (dtype: `float`, default: `(0,0,0)`)
 - `image`: (*N*,3) array of periodic image indexes (dtype: `int`, default: `(0,0,0)`)
 - `velocity`: (*N*,3) array of velocities (dtype: `float`, default: `(0,0,0)`)
 - `molecule`: (*N*,) array of molecule indexes (dtype: `int`, default: `0`)
 - `typeid`: (*N*,) array of type indexes (dtype: `int`, default: `1`)
 - `mass`: (*N*,) array of masses (dtype: `float`, default: `1`)
 - `charge`: (*N*,) array of charges (dtype: `float`, default: `0`)
+- `bonds`: Bond data (dtype: `Bonds`, default: `None`)
+- `angles`: Angle data (dtype: `Angles`, default: `None`)
+- `dihedrals`: Dihedral data (dtype: `Dihedrals`, default: `None`)
+- `impropers`: Improper data (dtype: `Impropers`, default: `None`)
 
 All values of indexes will follow the LAMMPS 1-indexed convention, but the
 arrays themselves are 0-indexed.
 
 The `Snapshot` will lazily initialize these per-particle arrays as they are
 accessed to save memory. Hence, accessing a per-particle property will allocate
 it to default values. If you want to check if an attribute has been set, use the
 corresponding `has_` method instead (e.g., `has_position()`):
 
     snapshot.position = [[0,0,0],[1,-1,1],[1.5,2.5,-3.5]]
     snapshot.typeid[2] = 2
     if not snapshot.has_mass():
         snapshot.mass = [2.,2.,10.]
 
+## Topology
+
+The topology (bond information) can be stored in `Bonds`, `Angles`, `Dihedrals`,
+and `Impropers` objects. All these objects function similarly, differing only in the
+number of particles that are included in a connection (2 for a bond, 3 for an angle,
+4 for a dihedral or improper). Each connection has an associated `id` and `typeid`.
+
+```py
+bonds = Bonds(N=3, num_types=2)
+angles = Angles(N=2, num_types=1)
+```
+These constructor arguments are available as attributes:
+
+- `N`: number of connections (int)
+- `num_types`: number of connection types (int). If `num_types is None`, then the number of types is deduced from `typeid`.
+
+The data contained per connection is:
+- `num_members`: (*N*, *M*) array of particles IDs in each topology (dtype: `int`, default: `1`),
+where *M* is the number of particles in a connection.
+- `id`: (*N*,) array topology IDs (dtype: `int`, default: runs from 1 to *N*)
+- `typeid`: (*N*,) array of type indexes (dtype: `int`, default: `1`)
+
+All values of indexes will follow the LAMMPS 1-indexed convention, but the
+arrays themselves are 0-indexed. Lazy array initialization is used as for the `Snapshot`.
+
 ## Data files
 
 A LAMMPS data file is represented by a `DataFile`. The file must be explicitly
 `read()` to get a `Snapshot`:
 
     f = lammpsio.DataFile("config.data")
     snapshot = f.read()
```

### Comparing `lammpsio-0.4.1/README.md` & `lammpsio-0.5.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -25,39 +25,69 @@
     snapshot = lammpsio.Snapshot(3, box, step=100)
 
 These constructor arguments are available as attributes:
 
 - `N`: number of particles (int)
 - `box`: bounding box (`Box`)
 - `step`: timestep counter (int)
+- `num_types`: number of particle types (int). If `num_types is None`, then the number of types is deduced from `typeid`.
 
 The data contained in a `Snapshot` per particle is:
 
 - `id`: (*N*,) array atom IDs (dtype: `int`, default: runs from 1 to *N*)
 - `position`: (*N*,3) array of coordinates (dtype: `float`, default: `(0,0,0)`)
 - `image`: (*N*,3) array of periodic image indexes (dtype: `int`, default: `(0,0,0)`)
 - `velocity`: (*N*,3) array of velocities (dtype: `float`, default: `(0,0,0)`)
 - `molecule`: (*N*,) array of molecule indexes (dtype: `int`, default: `0`)
 - `typeid`: (*N*,) array of type indexes (dtype: `int`, default: `1`)
 - `mass`: (*N*,) array of masses (dtype: `float`, default: `1`)
 - `charge`: (*N*,) array of charges (dtype: `float`, default: `0`)
+- `bonds`: Bond data (dtype: `Bonds`, default: `None`)
+- `angles`: Angle data (dtype: `Angles`, default: `None`)
+- `dihedrals`: Dihedral data (dtype: `Dihedrals`, default: `None`)
+- `impropers`: Improper data (dtype: `Impropers`, default: `None`)
 
 All values of indexes will follow the LAMMPS 1-indexed convention, but the
 arrays themselves are 0-indexed.
 
 The `Snapshot` will lazily initialize these per-particle arrays as they are
 accessed to save memory. Hence, accessing a per-particle property will allocate
 it to default values. If you want to check if an attribute has been set, use the
 corresponding `has_` method instead (e.g., `has_position()`):
 
     snapshot.position = [[0,0,0],[1,-1,1],[1.5,2.5,-3.5]]
     snapshot.typeid[2] = 2
     if not snapshot.has_mass():
         snapshot.mass = [2.,2.,10.]
 
+## Topology
+
+The topology (bond information) can be stored in `Bonds`, `Angles`, `Dihedrals`,
+and `Impropers` objects. All these objects function similarly, differing only in the
+number of particles that are included in a connection (2 for a bond, 3 for an angle,
+4 for a dihedral or improper). Each connection has an associated `id` and `typeid`.
+
+```py
+bonds = Bonds(N=3, num_types=2)
+angles = Angles(N=2, num_types=1)
+```
+These constructor arguments are available as attributes:
+
+- `N`: number of connections (int)
+- `num_types`: number of connection types (int). If `num_types is None`, then the number of types is deduced from `typeid`.
+
+The data contained per connection is:
+- `num_members`: (*N*, *M*) array of particles IDs in each topology (dtype: `int`, default: `1`),
+where *M* is the number of particles in a connection.
+- `id`: (*N*,) array topology IDs (dtype: `int`, default: runs from 1 to *N*)
+- `typeid`: (*N*,) array of type indexes (dtype: `int`, default: `1`)
+
+All values of indexes will follow the LAMMPS 1-indexed convention, but the
+arrays themselves are 0-indexed. Lazy array initialization is used as for the `Snapshot`.
+
 ## Data files
 
 A LAMMPS data file is represented by a `DataFile`. The file must be explicitly
 `read()` to get a `Snapshot`:
 
     f = lammpsio.DataFile("config.data")
     snapshot = f.read()
```

### Comparing `lammpsio-0.4.1/setup.cfg` & `lammpsio-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `lammpsio-0.4.1/src/lammpsio/box.py` & `lammpsio-0.5.0/src/lammpsio/box.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.4.1/src/lammpsio/data.py` & `lammpsio-0.5.0/src/lammpsio/dump.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,408 +1,397 @@
+import gzip
+import os
+import pathlib
+
 import numpy
 
 from .box import Box
+from .data import _readline
 from .snapshot import Snapshot
 
 
-def _readline(file_, require=False):
-    """Read and require a line."""
-    line = file_.readline()
-    if require and len(line) == 0:
-        raise OSError("Could not read line from file")
-    return line
+class DumpFile:
+    """LAMMPS dump file.
 
+    The dump file is a flexible file format, so a ``schema`` can be given
+    to parse the atom data. The ``schema`` is given as a dictionary of column
+    indexes. Valid keys for the schema match the names and shapes in the `Snapshot`.
+    The keys requiring only 1 column index are: ``id``, ``typeid``, ``molecule``,
+    ``charge``, and ``mass``. The keys requiring 3 column indexes are ``position``,
+    ``velocity``, and ``image``. If a ``schema`` is not specified, it will be deduced
+    from the ``ITEM: ATOMS`` header.
 
-class DataFile:
-    """LAMMPS data file.
+    The vector-valued fields (``position``, ``velocity``, ``image``) must contain all
+    three elements.
 
     Parameters
     ----------
     filename : str
-        Path to data file.
-    atom_style : str
-        Atom style to use for data file. Defaults to ``None``, which means the
-        style should be read from the file.
-
-    Attributes
-    ----------
-    filename : str
-        Path to the file.
-    atom_style : str
-        Atom style for the file.
-    known_headers : list
-        Data file headers that can be processed.
-    unknown_headers : list
-        Data file headers that will be ignored.
-    known_bodies : list
-        Data file body sections that can be processed.
-    unknown_bodies : list
-        Data file body sections that will be ignored.
+        Path to dump file.
+    schema : dict
+        Schema for the contents of the file. Defaults to ``None``, which means to read
+        it from the file.
+    sort_ids : bool
+        If true, sort the particles by ID in each snapshot.
+    copy_from : :class:`Snapshot`
+        If specified, copy fields that are missing in the dump file but are set in
+        a reference :class:`Snapshot`. The fields that can be copied are ``typeid``,
+        ``molecule``, ``charge``, and ``mass``.
 
     """
 
-    def __init__(self, filename, atom_style=None):
+    def __init__(self, filename, schema=None, sort_ids=True, copy_from=None):
         self.filename = filename
-        self.atom_style = atom_style
-
-    known_headers = ("atoms", "atom types", "xlo xhi", "ylo yhi", "zlo zhi", "xy xz yz")
-    unknown_headers = (
-        "bonds",
-        "angles",
-        "dihedrals",
-        "impropers",
-        "bond types",
-        "angle types",
-        "dihedral types",
-        "improper types",
-        "extra bond per atom",
-        "extra angle per atom",
-        "extra dihedral per atom",
-        "extra improper per atom",
-        "ellipsoids",
-        "lines",
-        "triangles",
-        "bodies",
-    )
-    known_bodies = ("Atoms", "Velocities", "Masses")
-    unknown_bodies = (
-        "Ellipsoids",
-        "Lines",
-        "Triangles",
-        "Bodies",
-        "Bonds",
-        "Angles",
-        "Dihedrals",
-        "Impropers",
-    )
+        self.schema = schema
+        self._frames = None
+        self.sort_ids = sort_ids
+        self.copy_from = copy_from
 
     @classmethod
-    def create(cls, filename, snapshot, atom_style=None):
-        """Create a LAMMPS data file from a snapshot.
+    def create(cls, filename, schema, snapshots):
+        """Create a LAMMPS dump file.
 
         Parameters
         ----------
         filename : str
-            Path to data file.
-        snapshot : :class:`Snapshot`
-            Snapshot to write to file.
-        atom_style : str
-            Atom style to use for data file. Defaults to ``None``, which means the
-            style should be inferred from the contents of ``snapshot``.
+            Path to dump file.
+        schema : dict
+            Schema for the contents of the file.
+        snapshots : :class:`Snapshot` or list
+            One or more snapshots to write to the dump file.
 
         Returns
         -------
-        :class:`DataFile`
-            The object representing the new data file.
-
-        Raises
-        ------
-        ValueError
-            If all masses are not the same for a given type.
+        :class:`DumpFile`
+            The object representing the new dump file.
 
         """
-        # extract number of types
-        num_types = numpy.amax(numpy.unique(snapshot.typeid))
-
-        # extract mass by type
-        if snapshot.has_mass():
-            masses = numpy.empty(num_types)
-            for i in range(num_types):
-                mi = snapshot.mass[snapshot.typeid == i + 1]
-                if not numpy.all(mi == mi[0]):
-                    raise ValueError("All masses for a type must be equal")
-                elif mi[0] <= 0.0:
-                    raise ValueError("Type mass must be positive value")
-                masses[i] = mi[0]
-        else:
-            masses = None
+        # map out the schema into a dump row
+        # each entry is a tuple: (column, (attribute, index))
+        # the index is None for scalars, otherwise it is the component of the vector
+        dump_row = []
+        for k, v in schema.items():
+            try:
+                cols = iter(v)
+                for i, col in enumerate(cols):
+                    dump_row.append((col, (k, i)))
+            except TypeError:
+                dump_row.append((v, (k, None)))
+        dump_row.sort(key=lambda x: x[0])
+
+        # make snapshots iterable
+        try:
+            snapshots = iter(snapshots)
+        except TypeError:
+            snapshots = [snapshots]
 
         with open(filename, "w") as f:
-            # LAMMPS header
-            f.write(
-                f"LAMMPS {filename}\n\n"
-                f"{snapshot.N} atoms\n"
-                f"{num_types} atom types\n"
-                f"{snapshot.box.low[0]} {snapshot.box.high[0]} xlo xhi\n"
-                f"{snapshot.box.low[1]} {snapshot.box.high[1]} ylo yhi\n"
-                f"{snapshot.box.low[2]} {snapshot.box.high[2]} zlo zhi\n"
-            )
-            if snapshot.box.tilt is not None:
-                f.write("{} {} {} xy xz yz\n".format(*snapshot.box.tilt))
-
-            # Atoms section
-            # determine style if it is not given
-            if atom_style is None:
-                if snapshot.has_charge() and snapshot.has_molecule():
-                    style = "full"
-                elif snapshot.has_charge():
-                    style = "charge"
-                elif snapshot.has_molecule():
-                    style = "molecular"
-                else:
-                    style = "atomic"
-            else:
-                style = atom_style
-            # set format string based on style
-            if style == "full":
-                style_fmt = (
-                    "{atomid:d} {molid:d} {typeid:d} {q:.5f} {x:.8f} {y:.8f} {z:.8f}"
-                )
-            elif style == "charge":
-                style_fmt = "{atomid:d} {typeid:d} {q:.5f} {x:.8f} {y:.8f} {z:.8f}"
-            elif style == "molecular":
-                style_fmt = "{atomid:d} {molid:d} {typeid:d} {x:.8f} {y:.8f} {z:.8f}"
-            elif style == "atomic":
-                style_fmt = "{atomid:d} {typeid:d} {x:.8f} {y:.8f} {z:.8f}"
-            else:
-                raise ValueError("Unknown atom style")
-            if snapshot.has_image():
-                style_fmt += " {ix:d} {iy:d} {iz:d}"
-            # write section
-            f.write(f"\nAtoms # {style}\n\n")
-            for i in range(snapshot.N):
-                style_args = dict(
-                    atomid=snapshot.id[i] if snapshot.has_id() else i + 1,
-                    typeid=snapshot.typeid[i],
-                    x=snapshot.position[i][0],
-                    y=snapshot.position[i][1],
-                    z=snapshot.position[i][2],
-                    q=snapshot.charge[i] if snapshot.has_charge() else 0.0,
-                    molid=snapshot.molecule[i] if snapshot.has_molecule() else 0,
-                )
-                if snapshot.has_image():
-                    style_args.update(
-                        ix=snapshot.image[i][0],
-                        iy=snapshot.image[i][1],
-                        iz=snapshot.image[i][2],
-                    )
-
-                f.write(style_fmt.format(**style_args) + "\n")
-
-            # Velocities section
-            if snapshot.has_velocity():
-                f.write("\nVelocities\n\n")
-                for i in range(snapshot.N):
-                    vel_fmt = "{atomid:8d}{vx:16.8f}{vy:16.8f}{vz:16.8f}\n"
-                    f.write(
-                        vel_fmt.format(
-                            atomid=snapshot.id[i] if snapshot.has_id() else i + 1,
-                            vx=snapshot.velocity[i][0],
-                            vy=snapshot.velocity[i][1],
-                            vz=snapshot.velocity[i][2],
-                        )
-                    )
-
-            # Masses section
-            if masses is not None:
-                f.write("\nMasses\n\n")
-                for i, mi in enumerate(masses):
-                    f.write("{typeid:4d}{m:12}\n".format(typeid=i + 1, m=mi))
+            for snap in snapshots:
+                f.write("ITEM: TIMESTEP\n" f"{snap.step}\n")
 
-        return DataFile(filename)
+                f.write("ITEM: NUMBER OF ATOMS\n")
+                f.write(f"{snap.N}\n")
 
-    def read(self):
-        """Read the file.
-
-        Returns
-        -------
-        :class:`Snapshot`
-            Snapshot from the data file.
+                # always assume periodic in all directions
+                box_header = "ITEM: BOX BOUNDS pp pp pp"
+                if snap.box.tilt is not None:
+                    xy, xz, yz = snap.box.tilt
+                    box_header += f" {xy:f} {xz:f} {yz:f}"
+                    lo = [
+                        snap.box.low[0] + min([0.0, xy, xz, xy + xz]),
+                        snap.box.low[1] + min([0.0, yz]),
+                        snap.box.low[2],
+                    ]
+                    hi = [
+                        snap.box.high[0] + max([0.0, xy, xz, xy + xz]),
+                        snap.box.high[1] + max([0.0, yz]),
+                        snap.box.high[2],
+                    ]
+                else:
+                    lo = snap.box.low
+                    hi = snap.box.high
+                f.write(box_header + "\n")
+                for i in range(3):
+                    f.write(f"{lo[i]:f} {hi[i]:f}\n")
+
+                # mapping from lammpsio to LAMMPS dump keys
+                lammps_fields = {
+                    "id": "id",
+                    "molecule": "mol",
+                    "typeid": "type",
+                    "mass": "mass",
+                    "position": ("x", "y", "z"),
+                    "image": ("ix", "iy", "iz"),
+                    "velocity": ("vx", "vy", "vz"),
+                    "charge": "q",
+                }
+                schema_header = []
+                for _, (key, key_idx) in dump_row:
+                    field = lammps_fields[key]
+                    if key_idx is not None:
+                        field = field[key_idx]
+                    schema_header.append(field)
+                schema_header = " ".join(schema_header)
+
+                f.write("ITEM: ATOMS " + schema_header + "\n")
+                for i in range(snap.N):
+                    line = ""
+                    for col, (key, key_idx) in dump_row:
+                        if key == "id":
+                            val = snap.id[i] if snap.has_id() else i + 1
+                        else:
+                            val = getattr(snap, key)[i]
+                            if key_idx is not None:
+                                val = val[key_idx]
+
+                        if key in ("id", "typeid", "molecule", "image"):
+                            fmt = "{:d}"
+                        elif key in ("position", "velocity"):
+                            fmt = "{:.8f}"
+                        else:
+                            fmt = "{:f}"
 
-        Raises
-        ------
-        ValueError
-            If :attr:`atom_style` is set but does not match file contents.
-        ValueError
-            If :attr:`atom_style` is not specified and not set in file.
+                        if col > 0:
+                            fmt = " " + fmt
+                        line += fmt.format(val)
+                    line = line.strip()
+                    f.write(line + "\n")
+
+        filename_path = pathlib.Path(filename)
+        if filename_path.suffix == ".gz":
+            tmp = pathlib.Path(filename).with_suffix(filename_path.suffix + ".tmp")
+            with open(filename, "rb") as src, gzip.open(tmp, "wb") as dest:
+                dest.writelines(src)
+            os.replace(tmp, filename)
+
+        return DumpFile(filename, schema)
+
+    @property
+    def copy_from(self):
+        return self._copy_from
+
+    @copy_from.setter
+    def copy_from(self, value):
+        if value is not None and not isinstance(value, Snapshot):
+            raise TypeError("Dump file can only copy from Snapshot")
+        self._copy_from = value
+
+    @property
+    def filename(self):
+        """str: Path to the file."""
+        return self._filename
+
+    @filename.setter
+    def filename(self, value):
+        self._filename = value
+        self._gzip = pathlib.Path(value).suffix == ".gz"
+
+        # configure section labels of dump file
+        self._section = {
+            "step": "ITEM: TIMESTEP",
+            "natoms": "ITEM: NUMBER OF ATOMS",
+            "box": "ITEM: BOX BOUNDS",
+            "atoms": "ITEM: ATOMS",
+        }
+        if self._gzip:
+            for key, val in self._section.items():
+                self._section[key] = val.encode()
+
+    @property
+    def schema(self):
+        """dict: Data schema."""
+        return self._schema
+
+    @schema.setter
+    def schema(self, value):
+        if value is not None:
+            # validate schema
+            if "position" in value and len(value["position"]) != 3:
+                raise ValueError("Position must be a 3-tuple")
+            if "velocity" in value and len(value["velocity"]) != 3:
+                raise ValueError("Velocity must be a 3-tuple")
+            if "image" in value and len(value["image"]) != 3:
+                raise ValueError("Image must be a 3-tuple")
+        self._schema = value
+
+    def _open(self):
+        """Open the file handle for reading."""
+        if self._gzip:
+            f = gzip.open(self.filename, "rb")
+        else:
+            f = open(self.filename, "r")
+        return f
 
-        """
-        with open(self.filename) as f:
-            # initialize snapshot from header
-            N = None
-            box_bounds = [None, None, None, None, None, None]
-            box_tilt = None
-            num_types = None
-            # skip first line
-            _readline(f, True)
+    def _find_frames(self):
+        """Seek line numbers for each frame."""
+        self._frames = []
+        with self._open() as f:
             line = _readline(f)
+            line_num = 0
             while len(line) > 0:
-                line = line.rstrip()
-
-                # skip blank and go to next line
-                if len(line) == 0:
-                    line = _readline(f)
-                    continue
-
-                # check for unknown headers and go to next line
-                skip_line = False
-                for h in self.unknown_headers:
-                    if h in line:
-                        skip_line = True
-                        break
-                if skip_line:
-                    line = _readline(f)
-                    continue
-
-                # line is not empty but it is not a header, so break and try to
-                # make snapshot keep the line so that it can be processed in
-                # next step
-                done_header = True
-                for h in self.known_headers:
-                    if h in line:
-                        done_header = False
-                        break
-                if done_header:
-                    break
-
-                # process useful header info
-                if "atoms" in line:
-                    N = int(line.split()[0])
-                elif "atom types" in line:
-                    num_types = int(line.split()[0])
-                elif "xlo xhi" in line:
-                    box_bounds[0], box_bounds[3] = [float(x) for x in line.split()[:2]]
-                elif "ylo yhi" in line:
-                    box_bounds[1], box_bounds[4] = [float(x) for x in line.split()[:2]]
-                elif "zlo zhi" in line:
-                    box_bounds[2], box_bounds[5] = [float(x) for x in line.split()[:2]]
-                elif "xy xz yz" in line:
-                    box_tilt = [float(x) for x in line.split()[:3]]
-                else:
-                    raise RuntimeError("Uncaught header line! Check programming")
-
-                # done here, read next line
+                if self._section["step"] in line:
+                    self._frames.append(line_num)
                 line = _readline(f)
+                line_num += 1
 
-            if N is None:
-                raise IOError("Number of particles not read")
-            elif num_types is None:
-                raise IOError("Number of types not read")
-            elif None in box_bounds:
-                raise IOError("Box bounds not read")
-            box = Box(box_bounds[:3], box_bounds[3:], box_tilt)
-            snap = Snapshot(N, box)
-            id_map = {}
-
-            # now that snapshot is made, file it in with body sections
-            masses = None
+    def __len__(self):
+        if self._frames is None:
+            self._find_frames()
+        return len(self._frames)
+
+    def __iter__(self):
+        with self._open() as f:
+            state = 0
+            line = _readline(f)
             while len(line) > 0:
-                if "Atoms" in line:
-                    # use or extract style
-                    row = line.split()
-                    if len(row) == 3:
-                        style = row[-1]
-                        if self.atom_style is not None and style != self.atom_style:
-                            raise ValueError(
-                                "Specified style does not match style in file"
-                            )
+                # timestep line first
+                if state == 0 and self._section["step"] in line:
+                    state += 1
+                    step = int(_readline(f, True))
+
+                # number of particles second
+                if state == 1 and self._section["natoms"] in line:
+                    state += 1
+                    N = int(_readline(f, True))
+
+                # box size third
+                if state == 2 and self._section["box"] in line:
+                    state += 1
+                    box_header = line.split()
+                    # check for triclinic
+                    if len(box_header) == 9:
+                        box_tilt = [float(x) for x in box_header[6:9]]
+                    elif len(box_header) == 6:
+                        box_tilt = None
                     else:
-                        style = self.atom_style
-                    if style is None:
-                        raise IOError("Atom style not found, specify.")
-                    # number of columns to read for style
-                    if style == "full":
-                        style_cols = 3
-                    elif style == "charge":
-                        style_cols = 2
-                    elif style == "molecular":
-                        style_cols = 2
-                    elif style == "atomic":
-                        style_cols = 1
+                        raise IOError("Incorrectly formed box bound header")
+                    box_x = _readline(f, True)
+                    box_y = _readline(f, True)
+                    box_z = _readline(f, True)
+                    x_lo, x_hi = [float(x) for x in box_x.split()]
+                    y_lo, y_hi = [float(y) for y in box_y.split()]
+                    z_lo, z_hi = [float(z) for z in box_z.split()]
+                    if box_tilt is not None:
+                        xy, xz, yz = box_tilt
+                        lo = [
+                            x_lo - min([0.0, xy, xz, xy + xz]),
+                            y_lo - min([0.0, yz]),
+                            z_lo,
+                        ]
+                        hi = [
+                            x_hi - max([0.0, xy, xz, xy + xz]),
+                            y_hi - max([0.0, yz]),
+                            z_hi,
+                        ]
+                        box = Box(lo, hi, box_tilt)
                     else:
-                        raise ValueError("Unknown atom style")
+                        box = Box([x_lo, y_lo, z_lo], [x_hi, y_hi, z_hi])
 
-                    # read atom coordinates
-                    _readline(f, True)  # blank line
-                    for i in range(snap.N):
-                        # strip out comments
-                        row = _readline(f, True).split()
-                        try:
-                            comment = row.index("#")
-                            row = row[:comment]
-                        except ValueError:
-                            pass
-
-                        # check that row is correctly sized and process
-                        if not (
-                            len(row) == style_cols + 4 or len(row) == style_cols + 7
-                        ):
-                            raise IOError(
-                                "Expected number of columns not read for atom style"
-                            )
+                # atoms come fourth
+                if state == 3 and self._section["atoms"] in line:
+                    state += 1
+
+                    # extract the scehma
+                    if self.schema is None:
+                        # mapping from LAMMPS dump keys to lammpsio
+                        lammps_fields = {
+                            "id": ("id", None),
+                            "mol": ("molecule", None),
+                            "type": ("typeid", None),
+                            "mass": ("mass", None),
+                            "x": ("position", 0),
+                            "y": ("position", 1),
+                            "z": ("position", 2),
+                            "ix": ("image", 0),
+                            "iy": ("image", 1),
+                            "iz": ("image", 2),
+                            "vx": ("velocity", 0),
+                            "vy": ("velocity", 1),
+                            "vz": ("velocity", 2),
+                            "q": ("charge", None),
+                        }
+                        schema = {}
+                        schema_header = line.split()[2:]
+                        for i, field in enumerate(schema_header):
+                            if self._gzip:
+                                field = field.decode()
+                            if field in lammps_fields:
+                                key, key_idx = lammps_fields[field]
+                                if key_idx is not None:
+                                    if key not in schema:
+                                        schema[key] = [None, None, None]
+                                    schema[key][key_idx] = i
+                                else:
+                                    schema[key] = i
+                        # validate tuple
+                        for key in ("position", "velocity", " image"):
+                            if key in schema and any(x is None for x in schema[key]):
+                                raise IOError("lammpsio requires 3-element vectors")
+                        self.schema = schema
 
-                        # only save the atom id if it is not in standard order
-                        id_ = int(row[0])
-                        if id_ != i + 1:
-                            if id_ not in id_map:
-                                id_map[id_] = i
-                            idx = id_map[id_]
-                            snap.id[idx] = id_
-                        else:
-                            idx = i
+                    snap = Snapshot(N, box, step)
+                    for i in range(snap.N):
+                        atom = _readline(f, True)
+                        atom = atom.split()
 
-                        if style == "full":
-                            snap.molecule[idx] = int(row[1])
-                            snap.typeid[idx] = int(row[2])
-                            snap.charge[idx] = float(row[3])
-                        elif style == "charge":
-                            snap.typeid[idx] = int(row[1])
-                            snap.charge[idx] = float(row[2])
-                        elif style == "molecular":
-                            snap.molecule[idx] = int(row[1])
-                            snap.typeid[idx] = int(row[2])
-                        elif style == "atomic":
-                            snap.typeid[idx] = int(row[1])
-                        snap.position[idx] = [
-                            float(x) for x in row[style_cols + 1 : style_cols + 4]
-                        ]
-                        if len(row) == style_cols + 7:
-                            snap.image[idx] = [
-                                int(x) for x in row[style_cols + 4 : style_cols + 7]
+                        if "id" in self.schema:
+                            id_ = int(atom[self.schema["id"]])
+                            if id_ != i + 1:
+                                snap.id[i] = id_
+                        if "position" in self.schema:
+                            snap.position[i] = [
+                                float(atom[j]) for j in self.schema["position"]
                             ]
-
-                    # sanity check types
-                    if numpy.any(
-                        numpy.logical_or(snap.typeid < 1, snap.typeid > num_types)
-                    ):
-                        raise ValueError("Invalid type id")
-                elif "Velocities" in line:
-                    _readline(f, True)  # blank line
-                    for i in range(snap.N):
-                        row = _readline(f, True).split()
-                        if len(row) < 4:
-                            raise IOError(
-                                "Expected number of columns not read for velocity"
+                        if "velocity" in self.schema:
+                            snap.velocity[i] = [
+                                float(atom[j]) for j in self.schema["velocity"]
+                            ]
+                        if "image" in self.schema:
+                            snap.image[i] = [int(atom[j]) for j in self.schema["image"]]
+                        if "molecule" in self.schema:
+                            snap.molecule[i] = int(atom[self.schema["molecule"]])
+                        if "typeid" in self.schema:
+                            snap.typeid[i] = int(atom[self.schema["typeid"]])
+                        if "charge" in self.schema:
+                            snap.charge[i] = float(atom[self.schema["charge"]])
+                        if "mass" in self.schema:
+                            snap.mass[i] = float(atom[self.schema["mass"]])
+
+                # final processing stage for the frame
+                if state == 4:
+                    # optionally sort the particles by ID
+                    if self.sort_ids and snap.has_id():
+                        snap.reorder(numpy.argsort(snap.id), check_order=False)
+
+                    # optionally copy reference data by ID / index
+                    if self._copy_from is not None:
+                        if snap.N != self._copy_from.N:
+                            raise ValueError(
+                                "Cannot copy from a Snapshot with a different size"
                             )
-                        # parse atom id: need to repeat mapping in case
-                        # Velocity comes before Atoms
-                        id_ = int(row[0])
-                        if id_ != i + 1:
-                            if id_ not in id_map:
-                                id_map[id_] = i
-                            idx = id_map[id_]
-                            snap.id[idx] = id_
+
+                        if self._copy_from.has_id():
+                            copy_id_map = {
+                                id_: i for i, id_ in enumerate(self._copy_from.id)
+                            }
                         else:
-                            idx = i
-                        snap.velocity[idx] = [float(x) for x in row[1:4]]
-                elif "Masses" in line:
-                    masses = {}
-                    _readline(f, True)  # blank line
-                    for i in range(num_types):
-                        row = _readline(f, True).split()
-                        if len(row) < 2:
-                            raise IOError(
-                                "Expected number of columns not read for mass"
-                            )
-                        masses[int(row[0])] = float(row[1])
-                else:
-                    # silently ignore unknown sections / lines
-                    pass
+                            copy_id_map = {i + 1: i for i in range(self._copy_from.N)}
 
-                line = _readline(f)
+                        if snap.has_id():
+                            copy_id = [copy_id_map[id_] for id_ in snap.id]
+                        else:
+                            copy_id = [copy_id_map[id_] for id_ in range(1, snap.N + 1)]
 
-            # set mass on particles at end, in case sections were out of order in file
-            if masses is not None:
-                for typeid, m in masses.items():
-                    snap.mass[snap.typeid == typeid] = m
+                        if not snap.has_typeid() and self._copy_from.has_typeid():
+                            snap.typeid = self._copy_from.typeid[copy_id]
+                        if not snap.has_molecule() and self._copy_from.has_molecule():
+                            snap.molecule = self._copy_from.molecule[copy_id]
+                        if not snap.has_charge() and self._copy_from.has_charge():
+                            snap.charge = self._copy_from.charge[copy_id]
+                        if not snap.has_mass() and self._copy_from.has_mass():
+                            snap.mass = self._copy_from.mass[copy_id]
+
+                    yield snap
+                    del snap, N, box, step
+                    state = 0
 
-        return snap
+                line = _readline(f)
```

### Comparing `lammpsio-0.4.1/src/lammpsio/snapshot.py` & `lammpsio-0.5.0/src/lammpsio/snapshot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import warnings
 
 import numpy
 import packaging.version
 
 from .box import Box
+from .topology import Angles, Bonds, Dihedrals, Impropers
 
 _optional_imports = set()
 try:
     import gsd
     import gsd.hoomd
 
     _optional_imports.add("gsd")
@@ -31,27 +32,32 @@
     Attributes
     ----------
     step : int
         Simulation time step counter.
 
     """
 
-    def __init__(self, N, box, step=None):
+    def __init__(self, N, box, step=None, num_types=None):
         self._N = N
         self._box = Box.cast(box)
         self.step = step
 
         self._id = None
         self._position = None
         self._velocity = None
         self._image = None
         self._molecule = None
+        self._num_types = None
         self._typeid = None
         self._charge = None
         self._mass = None
+        self._bonds = None
+        self._angles = None
+        self._dihedrals = None
+        self._impropers = None
 
     @classmethod
     def from_hoomd_gsd(cls, frame):
         """Create from a HOOMD GSD frame.
 
         Parameters
         ----------
@@ -94,14 +100,21 @@
         snap.charge = frame.particles.charge
         snap.mass = frame.particles.mass
 
         snap.molecule = frame.particles.body + 1
         if numpy.any(snap.molecule < 0):
             warnings.warn("Some molecule IDs are negative, remapping needed.")
 
+        if (
+            frame.bonds.N > 0
+            or frame.angles.N > 0
+            or frame.dihedrals.N > 0
+            or frame.impropers.N > 0
+        ):
+            warnings.warn("Conversion of topology from gsd is not supported")
         type_map = {typeid + 1: i for typeid, i in enumerate(frame.particles.types)}
 
         return snap, type_map
 
     def to_hoomd_gsd(self, type_map=None):
         """Create a HOOMD GSD frame.
 
@@ -181,14 +194,22 @@
         if self.has_molecule():
             frame.particles.body = self.molecule - 1
 
         # undo the sort so object goes back the way it was
         if reverse_order is not None:
             self.reorder(reverse_order, check_order=False)
 
+        if (
+            self.has_bonds()
+            or self.has_angles()
+            or self.has_dihedrals()
+            or self.has_impropers()
+        ):
+            warnings.warn("Conversion of topology to gsd is not supported")
+
         return frame
 
     @property
     def N(self):
         """int: Number of particles."""
         return self._N
 
@@ -344,14 +365,32 @@
         bool
             True if molecule tags have been initialized.
 
         """
         return self._molecule is not None
 
     @property
+    def num_types(self):
+        """int: Number of atom types."""
+        if self._num_types is not None:
+            return self._num_types
+        else:
+            if self.has_typeid():
+                return numpy.amax(self.typeid)
+            else:
+                return 1
+
+    @num_types.setter
+    def num_types(self, value):
+        if value is not None:
+            self._num_types = int(value)
+        else:
+            self._num_types = None
+
+    @property
     def typeid(self):
         """:class:`numpy.ndarray`: Types."""
         if not self.has_typeid():
             self._typeid = numpy.ones(self.N, dtype=int)
         return self._typeid
 
     @typeid.setter
@@ -433,14 +472,114 @@
         -------
         bool
             True if masses have been initialized.
 
         """
         return self._mass is not None
 
+    @property
+    def bonds(self):
+        """Bonds: Bond data."""
+        return self._bonds
+
+    @bonds.setter
+    def bonds(self, value):
+        if value is not None:
+            if not isinstance(value, Bonds):
+                raise TypeError("bonds must be Bonds")
+            self._bonds = value
+        else:
+            self._bonds = None
+
+    def has_bonds(self):
+        """Check if configuration has bonds.
+
+        Returns
+        -------
+        bool
+            True if bonds is initialized and there is at least one bond.
+
+        """
+        return self._bonds is not None and self._bonds.N > 0
+
+    @property
+    def angles(self):
+        """Angles: Angle data."""
+        return self._angles
+
+    @angles.setter
+    def angles(self, value):
+        if value is not None:
+            if not isinstance(value, Angles):
+                raise TypeError("angles must be Angles")
+            self._angles = value
+        else:
+            self._angles = None
+
+    def has_angles(self):
+        """Check if configuration has angles.
+
+        Returns
+        -------
+        bool
+            True if angles is initialized and there is at least one angle.
+
+        """
+        return self._angles is not None and self._angles.N > 0
+
+    @property
+    def dihedrals(self):
+        """Dihedrals: Dihedral data."""
+        return self._dihedrals
+
+    @dihedrals.setter
+    def dihedrals(self, value):
+        if value is not None:
+            if not isinstance(value, Dihedrals):
+                raise TypeError("dihedrals must be Dihedrals")
+            self._dihedrals = value
+        else:
+            self._dihedrals = None
+
+    def has_dihedrals(self):
+        """Check if configuration has dihedrals.
+
+        Returns
+        -------
+        bool
+            True if dihedrals is initialized and there is at least one dihedral.
+
+        """
+        return self._dihedrals is not None and self._dihedrals.N > 0
+
+    @property
+    def impropers(self):
+        """Impropers: Improper data."""
+        return self._impropers
+
+    @impropers.setter
+    def impropers(self, value):
+        if value is not None:
+            if not isinstance(value, Impropers):
+                raise TypeError("impropers must be Impropers")
+            self._impropers = value
+        else:
+            self._impropers = None
+
+    def has_impropers(self):
+        """Check if configuration has impropers.
+
+        Returns
+        -------
+        bool
+            True if impropers is initialized and there is at least one improper.
+
+        """
+        return self._impropers is not None and self._impropers.N > 0
+
     def reorder(self, order, check_order=True):
         """Reorder the particles in place.
 
         Parameters
         ----------
         order : list
             New order of indexes.
```

### Comparing `lammpsio-0.4.1/src/lammpsio.egg-info/PKG-INFO` & `lammpsio-0.5.0/src/lammpsio.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammpsio
-Version: 0.4.1
+Version: 0.5.0
 Summary: Python tools for working with LAMMPS
 Home-page: https://github.com/mphowardlab/lammpsio
 Author: Michael P. Howard
 Author-email: mphoward@auburn.edu
 Project-URL: Source Code, https://github.com/mphowardlab/lammpsio
 Project-URL: Issue Tracker, https://github.com/mphowardlab/lammpsio/issues
 Classifier: Intended Audience :: Science/Research
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: packaging
 
 # lammpsio
 
 [![PyPI version](https://img.shields.io/pypi/v/lammpsio.svg)](https://pypi.org/project/lammpsio)
 [![PyPI downloads](https://img.shields.io/pypi/dm/lammpsio)](https://pypi.org/project/lammpsio)
 [![Conda](https://img.shields.io/conda/dn/conda-forge/lammpsio)](https://anaconda.org/conda-forge/lammpsio)
 
@@ -46,39 +48,69 @@
     snapshot = lammpsio.Snapshot(3, box, step=100)
 
 These constructor arguments are available as attributes:
 
 - `N`: number of particles (int)
 - `box`: bounding box (`Box`)
 - `step`: timestep counter (int)
+- `num_types`: number of particle types (int). If `num_types is None`, then the number of types is deduced from `typeid`.
 
 The data contained in a `Snapshot` per particle is:
 
 - `id`: (*N*,) array atom IDs (dtype: `int`, default: runs from 1 to *N*)
 - `position`: (*N*,3) array of coordinates (dtype: `float`, default: `(0,0,0)`)
 - `image`: (*N*,3) array of periodic image indexes (dtype: `int`, default: `(0,0,0)`)
 - `velocity`: (*N*,3) array of velocities (dtype: `float`, default: `(0,0,0)`)
 - `molecule`: (*N*,) array of molecule indexes (dtype: `int`, default: `0`)
 - `typeid`: (*N*,) array of type indexes (dtype: `int`, default: `1`)
 - `mass`: (*N*,) array of masses (dtype: `float`, default: `1`)
 - `charge`: (*N*,) array of charges (dtype: `float`, default: `0`)
+- `bonds`: Bond data (dtype: `Bonds`, default: `None`)
+- `angles`: Angle data (dtype: `Angles`, default: `None`)
+- `dihedrals`: Dihedral data (dtype: `Dihedrals`, default: `None`)
+- `impropers`: Improper data (dtype: `Impropers`, default: `None`)
 
 All values of indexes will follow the LAMMPS 1-indexed convention, but the
 arrays themselves are 0-indexed.
 
 The `Snapshot` will lazily initialize these per-particle arrays as they are
 accessed to save memory. Hence, accessing a per-particle property will allocate
 it to default values. If you want to check if an attribute has been set, use the
 corresponding `has_` method instead (e.g., `has_position()`):
 
     snapshot.position = [[0,0,0],[1,-1,1],[1.5,2.5,-3.5]]
     snapshot.typeid[2] = 2
     if not snapshot.has_mass():
         snapshot.mass = [2.,2.,10.]
 
+## Topology
+
+The topology (bond information) can be stored in `Bonds`, `Angles`, `Dihedrals`,
+and `Impropers` objects. All these objects function similarly, differing only in the
+number of particles that are included in a connection (2 for a bond, 3 for an angle,
+4 for a dihedral or improper). Each connection has an associated `id` and `typeid`.
+
+```py
+bonds = Bonds(N=3, num_types=2)
+angles = Angles(N=2, num_types=1)
+```
+These constructor arguments are available as attributes:
+
+- `N`: number of connections (int)
+- `num_types`: number of connection types (int). If `num_types is None`, then the number of types is deduced from `typeid`.
+
+The data contained per connection is:
+- `num_members`: (*N*, *M*) array of particles IDs in each topology (dtype: `int`, default: `1`),
+where *M* is the number of particles in a connection.
+- `id`: (*N*,) array topology IDs (dtype: `int`, default: runs from 1 to *N*)
+- `typeid`: (*N*,) array of type indexes (dtype: `int`, default: `1`)
+
+All values of indexes will follow the LAMMPS 1-indexed convention, but the
+arrays themselves are 0-indexed. Lazy array initialization is used as for the `Snapshot`.
+
 ## Data files
 
 A LAMMPS data file is represented by a `DataFile`. The file must be explicitly
 `read()` to get a `Snapshot`:
 
     f = lammpsio.DataFile("config.data")
     snapshot = f.read()
```

### Comparing `lammpsio-0.4.1/tests/test_box.py` & `lammpsio-0.5.0/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.4.1/tests/test_dump_file.py` & `lammpsio-0.5.0/tests/test_dump_file.py`

 * *Files identical despite different names*

### Comparing `lammpsio-0.4.1/tests/test_snapshot.py` & `lammpsio-0.5.0/tests/test_snapshot.py`

 * *Files 15% similar despite different names*

```diff
@@ -156,14 +156,97 @@
     mass = [2, 3, 2]
     snap.mass = mass
     assert numpy.allclose(snap.mass, mass)
     with pytest.raises(TypeError):
         snap.mass = [1, 1]
 
 
+def test_bonds(snap_8):
+    snap_8.bonds = lammpsio.topology.Bonds(N=6, num_types=2)
+    id = [1, 2, 3, 4, 5, 6]
+    typeid = [1, 2, 1, 2, 1, 2]
+    members = [
+        [1, 2],
+        [2, 3],
+        [3, 4],
+        [5, 6],
+        [6, 7],
+        [7, 8],
+    ]
+
+    snap_8.bonds.id = id
+    snap_8.bonds.typeid = typeid
+    snap_8.bonds.members = members
+
+    assert numpy.allclose(snap_8.bonds.id, id)
+    assert numpy.allclose(snap_8.bonds.typeid, typeid)
+    assert numpy.allclose(snap_8.bonds.members, members)
+
+
+def test_angles(snap_8):
+    snap_8.angles = lammpsio.topology.Angles(N=4, num_types=2)
+    id = [
+        1,
+        2,
+        3,
+        4,
+    ]
+    typeid = [1, 2, 1, 2]
+    members = [
+        [1, 2, 3],
+        [2, 3, 4],
+        [5, 6, 7],
+        [6, 7, 8],
+    ]
+
+    snap_8.angles.id = id
+    snap_8.angles.typeid = typeid
+    snap_8.angles.members = members
+
+    assert numpy.allclose(snap_8.angles.id, id)
+    assert numpy.allclose(snap_8.angles.typeid, typeid)
+    assert numpy.allclose(snap_8.angles.members, members)
+
+
+def test_dihedrals(snap_8):
+    snap_8.dihedrals = lammpsio.topology.Dihedrals(N=2, num_types=2)
+    id = [1, 2]
+    typeid = [1, 2]
+    members = [
+        [1, 2, 3, 4],
+        [5, 6, 7, 8],
+    ]
+
+    snap_8.dihedrals.id = id
+    snap_8.dihedrals.typeid = typeid
+    snap_8.dihedrals.members = members
+
+    assert numpy.allclose(snap_8.dihedrals.id, id)
+    assert numpy.allclose(snap_8.dihedrals.typeid, typeid)
+    assert numpy.allclose(snap_8.dihedrals.members, members)
+
+
+def test_impropers(snap_8):
+    snap_8.impropers = lammpsio.topology.Impropers(N=2, num_types=2)
+    id = [1, 2]
+    typeid = [1, 2]
+    members = [
+        [1, 2, 3, 4],
+        [5, 6, 7, 8],
+    ]
+
+    snap_8.impropers.id = id
+    snap_8.impropers.typeid = typeid
+    snap_8.impropers.members = members
+
+    assert numpy.allclose(snap_8.impropers.id, id)
+    assert numpy.allclose(snap_8.impropers.typeid, typeid)
+    assert numpy.allclose(snap_8.impropers.members, members)
+
+
 def test_charge(snap):
     assert not snap.has_charge()
     assert numpy.allclose(snap.charge, 0)
     charge = [-1, 0, 1]
     snap.charge = charge
     assert numpy.allclose(snap.charge, charge)
     with pytest.raises(TypeError):
```

