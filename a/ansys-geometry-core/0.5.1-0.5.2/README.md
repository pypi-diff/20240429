# Comparing `tmp/ansys_geometry_core-0.5.1.tar.gz` & `tmp/ansys_geometry_core-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_geometry_core-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_geometry_core-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_geometry_core-0.5.1.tar` & `ansys_geometry_core-0.5.2.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0     1098 2024-04-24 15:03:14.635642 ansys_geometry_core-0.5.1/LICENSE
--rw-r--r--   0        0        0     5051 2024-04-24 15:03:14.635642 ansys_geometry_core-0.5.1/README.rst
--rw-r--r--   0        0        0     4373 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2762 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/__init__.py
--rw-r--r--   0        0        0     2477 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/__init__.py
--rw-r--r--   0        0        0     1618 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/backend.py
--rw-r--r--   0        0        0    12286 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/client.py
--rw-r--r--   0        0        0    18876 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/conversions.py
--rw-r--r--   0        0        0     2483 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/defaults.py
--rw-r--r--   0        0        0    13911 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/docker_instance.py
--rw-r--r--   0        0        0    28217 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/launcher.py
--rw-r--r--   0        0        0      167 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/pim_configuration.json
--rw-r--r--   0        0        0    16343 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/product_instance.py
--rw-r--r--   0        0        0     1776 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/validate.py
--rw-r--r--   0        0        0     1782 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/__init__.py
--rw-r--r--   0        0        0     7898 2024-04-24 15:03:14.639642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/beam.py
--rw-r--r--   0        0        0    46126 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/body.py
--rw-r--r--   0        0        0    52507 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/component.py
--rw-r--r--   0        0        0     6034 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/coordinate_system.py
--rw-r--r--   0        0        0    40126 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/design.py
--rw-r--r--   0        0        0     3697 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/designpoint.py
--rw-r--r--   0        0        0     6069 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/edge.py
--rw-r--r--   0        0        0    13956 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/face.py
--rw-r--r--   0        0        0     5468 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/part.py
--rw-r--r--   0        0        0     4686 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/selection.py
--rw-r--r--   0        0        0     4101 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/errors.py
--rw-r--r--   0        0        0    22524 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/logger.py
--rw-r--r--   0        0        0     1349 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/materials/__init__.py
--rw-r--r--   0        0        0     3268 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/materials/material.py
--rw-r--r--   0        0        0     4107 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/materials/property.py
--rw-r--r--   0        0        0     1883 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/__init__.py
--rw-r--r--   0        0        0     6819 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/bbox.py
--rw-r--r--   0        0        0     3259 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/constants.py
--rw-r--r--   0        0        0     7035 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/frame.py
--rw-r--r--   0        0        0     4823 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/matrix.py
--rw-r--r--   0        0        0     4240 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/plane.py
--rw-r--r--   0        0        0    12120 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/point.py
--rw-r--r--   0        0        0    18024 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/vector.py
--rw-r--r--   0        0        0     2085 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/__init__.py
--rw-r--r--   0        0        0     8033 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/accuracy.py
--rw-r--r--   0        0        0     5215 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/auxiliary.py
--rw-r--r--   0        0        0    12745 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/checks.py
--rw-r--r--   0        0        0     8253 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/measurements.py
--rw-r--r--   0        0        0     2291 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/options.py
--rw-r--r--   0        0        0     3684 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/units.py
--rw-r--r--   0        0        0    17075 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/modeler.py
--rw-r--r--   0        0        0     1417 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/__init__.py
--rw-r--r--   0        0        0    22177 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/plotter.py
--rw-r--r--   0        0        0    15007 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/plotter_helper.py
--rw-r--r--   0        0        0     5826 2024-04-24 15:03:14.643642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/plotting_types.py
--rw-r--r--   0        0        0     4213 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/trame_gui.py
--rw-r--r--   0        0        0     1710 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/__init__.py
--rw-r--r--   0        0        0      499 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/+xy.png
--rw-r--r--   0        0        0      487 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/+xz.png
--rw-r--r--   0        0        0      497 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/+yz.png
--rw-r--r--   0        0        0      496 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/-xy.png
--rw-r--r--   0        0        0      484 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/-xz.png
--rw-r--r--   0        0        0      495 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/-yz.png
--rw-r--r--   0        0        0      569 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png
--rw-r--r--   0        0        0      526 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png
--rw-r--r--   0        0        0      725 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/isometric.png
--rw-r--r--   0        0        0      339 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/measurement.png
--rw-r--r--   0        0        0      341 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/ruler.png
--rw-r--r--   0        0        0      451 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/upxarrow.png
--rw-r--r--   0        0        0      442 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/upyarrow.png
--rw-r--r--   0        0        0      428 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/upzarrow.png
--rw-r--r--   0        0        0     3058 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/button.py
--rw-r--r--   0        0        0     4239 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/displace_arrows.py
--rw-r--r--   0        0        0     3626 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/measure.py
--rw-r--r--   0        0        0     3700 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/ruler.py
--rw-r--r--   0        0        0     3480 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/show_design_point.py
--rw-r--r--   0        0        0     3348 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/view_button.py
--rw-r--r--   0        0        0     2305 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/widget.py
--rw-r--r--   0        0        0     2176 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/__init__.py
--rw-r--r--   0        0        0     5634 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/box_uv.py
--rw-r--r--   0        0        0     1580 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/__init__.py
--rw-r--r--   0        0        0    11617 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/circle.py
--rw-r--r--   0        0        0     3539 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/curve.py
--rw-r--r--   0        0        0     2767 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/curve_evaluation.py
--rw-r--r--   0        0        0    14319 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/ellipse.py
--rw-r--r--   0        0        0     8893 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/line.py
--rw-r--r--   0        0        0     7428 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/trimmed_curve.py
--rw-r--r--   0        0        0    13001 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/parameterization.py
--rw-r--r--   0        0        0     1746 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/__init__.py
--rw-r--r--   0        0        0    14274 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/cone.py
--rw-r--r--   0        0        0    14748 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/cylinder.py
--rw-r--r--   0        0        0     8067 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/plane.py
--rw-r--r--   0        0        0    13257 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/sphere.py
--rw-r--r--   0        0        0     3467 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/surface.py
--rw-r--r--   0        0        0     4281 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py
--rw-r--r--   0        0        0    16027 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/torus.py
--rw-r--r--   0        0        0     5694 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py
--rw-r--r--   0        0        0     1909 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/__init__.py
--rw-r--r--   0        0        0    11643 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/arc.py
--rw-r--r--   0        0        0     6690 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/box.py
--rw-r--r--   0        0        0     5139 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/circle.py
--rw-r--r--   0        0        0     2991 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/edge.py
--rw-r--r--   0        0        0     7734 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/ellipse.py
--rw-r--r--   0        0        0     3018 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/face.py
--rw-r--r--   0        0        0    19590 2024-04-24 15:03:14.647642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/gears.py
--rw-r--r--   0        0        0     6063 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/polygon.py
--rw-r--r--   0        0        0     6076 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/segment.py
--rw-r--r--   0        0        0    31342 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/sketch.py
--rw-r--r--   0        0        0     6878 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/slot.py
--rw-r--r--   0        0        0     8286 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/trapezoid.py
--rw-r--r--   0        0        0     3847 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/triangle.py
--rw-r--r--   0        0        0     1550 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/__init__.py
--rw-r--r--   0        0        0     3856 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/measurement_tools.py
--rw-r--r--   0        0        0    14367 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/problem_areas.py
--rw-r--r--   0        0        0     2429 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/repair_tool_message.py
--rw-r--r--   0        0        0    10524 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/repair_tools.py
--rw-r--r--   0        0        0     1670 2024-04-24 15:03:14.651642 ansys_geometry_core-0.5.1/src/ansys/geometry/core/typing.py
--rw-r--r--   0        0        0     9167 1970-01-01 00:00:00.000000 ansys_geometry_core-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-29 07:42:31.444221 ansys_geometry_core-0.5.2/LICENSE
+-rw-r--r--   0        0        0     4966 2024-04-29 07:42:31.444221 ansys_geometry_core-0.5.2/README.rst
+-rw-r--r--   0        0        0     4465 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2762 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/__init__.py
+-rw-r--r--   0        0        0     2477 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/__init__.py
+-rw-r--r--   0        0        0     1618 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/backend.py
+-rw-r--r--   0        0        0    12290 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/client.py
+-rw-r--r--   0        0        0    18876 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/conversions.py
+-rw-r--r--   0        0        0     2483 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/defaults.py
+-rw-r--r--   0        0        0    13911 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/docker_instance.py
+-rw-r--r--   0        0        0    28217 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/launcher.py
+-rw-r--r--   0        0        0      167 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/pim_configuration.json
+-rw-r--r--   0        0        0    16343 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/product_instance.py
+-rw-r--r--   0        0        0     1776 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/validate.py
+-rw-r--r--   0        0        0     1782 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/__init__.py
+-rw-r--r--   0        0        0     7898 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/beam.py
+-rw-r--r--   0        0        0    46126 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/body.py
+-rw-r--r--   0        0        0    52507 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/component.py
+-rw-r--r--   0        0        0     6034 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/coordinate_system.py
+-rw-r--r--   0        0        0    40126 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/design.py
+-rw-r--r--   0        0        0     3697 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/designpoint.py
+-rw-r--r--   0        0        0     6553 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/edge.py
+-rw-r--r--   0        0        0    14993 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/face.py
+-rw-r--r--   0        0        0     5468 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/part.py
+-rw-r--r--   0        0        0     4686 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/selection.py
+-rw-r--r--   0        0        0     4101 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/errors.py
+-rw-r--r--   0        0        0    22524 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/logger.py
+-rw-r--r--   0        0        0     1349 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/materials/__init__.py
+-rw-r--r--   0        0        0     3268 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/materials/material.py
+-rw-r--r--   0        0        0     4107 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/materials/property.py
+-rw-r--r--   0        0        0     1883 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/__init__.py
+-rw-r--r--   0        0        0     6819 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/bbox.py
+-rw-r--r--   0        0        0     3259 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/constants.py
+-rw-r--r--   0        0        0     7035 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/frame.py
+-rw-r--r--   0        0        0     4823 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/matrix.py
+-rw-r--r--   0        0        0     4240 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/plane.py
+-rw-r--r--   0        0        0    12120 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/point.py
+-rw-r--r--   0        0        0    18024 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/vector.py
+-rw-r--r--   0        0        0     2085 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/misc/__init__.py
+-rw-r--r--   0        0        0     8033 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/misc/accuracy.py
+-rw-r--r--   0        0        0     5215 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/misc/auxiliary.py
+-rw-r--r--   0        0        0    12751 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/misc/checks.py
+-rw-r--r--   0        0        0     8253 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/misc/measurements.py
+-rw-r--r--   0        0        0     2291 2024-04-29 07:42:31.452221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/misc/options.py
+-rw-r--r--   0        0        0     3684 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/misc/units.py
+-rw-r--r--   0        0        0    17075 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/modeler.py
+-rw-r--r--   0        0        0     1417 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/__init__.py
+-rw-r--r--   0        0        0    22177 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/plotter.py
+-rw-r--r--   0        0        0    15007 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/plotter_helper.py
+-rw-r--r--   0        0        0     5826 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/plotting_types.py
+-rw-r--r--   0        0        0     4213 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/trame_gui.py
+-rw-r--r--   0        0        0     1710 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/+xy.png
+-rw-r--r--   0        0        0      487 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/+xz.png
+-rw-r--r--   0        0        0      497 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/+yz.png
+-rw-r--r--   0        0        0      496 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/-xy.png
+-rw-r--r--   0        0        0      484 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/-xz.png
+-rw-r--r--   0        0        0      495 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/-yz.png
+-rw-r--r--   0        0        0      569 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png
+-rw-r--r--   0        0        0      526 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png
+-rw-r--r--   0        0        0      725 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/isometric.png
+-rw-r--r--   0        0        0      339 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/measurement.png
+-rw-r--r--   0        0        0      341 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/ruler.png
+-rw-r--r--   0        0        0      451 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/upxarrow.png
+-rw-r--r--   0        0        0      442 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/upyarrow.png
+-rw-r--r--   0        0        0      428 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/upzarrow.png
+-rw-r--r--   0        0        0     3058 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/button.py
+-rw-r--r--   0        0        0     4239 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/displace_arrows.py
+-rw-r--r--   0        0        0     3626 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/measure.py
+-rw-r--r--   0        0        0     3700 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/ruler.py
+-rw-r--r--   0        0        0     3480 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/show_design_point.py
+-rw-r--r--   0        0        0     3348 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/view_button.py
+-rw-r--r--   0        0        0     2305 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/widget.py
+-rw-r--r--   0        0        0     2176 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/__init__.py
+-rw-r--r--   0        0        0     5634 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/box_uv.py
+-rw-r--r--   0        0        0     1580 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/curves/__init__.py
+-rw-r--r--   0        0        0    11617 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/curves/circle.py
+-rw-r--r--   0        0        0     3539 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/curves/curve.py
+-rw-r--r--   0        0        0     2767 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/curves/curve_evaluation.py
+-rw-r--r--   0        0        0    14319 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/curves/ellipse.py
+-rw-r--r--   0        0        0     8893 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/curves/line.py
+-rw-r--r--   0        0        0     7428 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/curves/trimmed_curve.py
+-rw-r--r--   0        0        0    13001 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/parameterization.py
+-rw-r--r--   0        0        0     1746 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/__init__.py
+-rw-r--r--   0        0        0    14274 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/cone.py
+-rw-r--r--   0        0        0    14748 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/cylinder.py
+-rw-r--r--   0        0        0     8067 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/plane.py
+-rw-r--r--   0        0        0    13257 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/sphere.py
+-rw-r--r--   0        0        0     3467 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/surface.py
+-rw-r--r--   0        0        0     4281 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py
+-rw-r--r--   0        0        0    16027 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/torus.py
+-rw-r--r--   0        0        0     5694 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py
+-rw-r--r--   0        0        0     1909 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/__init__.py
+-rw-r--r--   0        0        0    11643 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/arc.py
+-rw-r--r--   0        0        0     6690 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/box.py
+-rw-r--r--   0        0        0     5139 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/circle.py
+-rw-r--r--   0        0        0     2991 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/edge.py
+-rw-r--r--   0        0        0     7734 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/ellipse.py
+-rw-r--r--   0        0        0     3018 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/face.py
+-rw-r--r--   0        0        0    19590 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/gears.py
+-rw-r--r--   0        0        0     6063 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/polygon.py
+-rw-r--r--   0        0        0     6076 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/segment.py
+-rw-r--r--   0        0        0    31342 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/sketch.py
+-rw-r--r--   0        0        0     6878 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/slot.py
+-rw-r--r--   0        0        0     8286 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/trapezoid.py
+-rw-r--r--   0        0        0     3847 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/triangle.py
+-rw-r--r--   0        0        0     1550 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/tools/__init__.py
+-rw-r--r--   0        0        0     3856 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/tools/measurement_tools.py
+-rw-r--r--   0        0        0    14367 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/tools/problem_areas.py
+-rw-r--r--   0        0        0     2429 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/tools/repair_tool_message.py
+-rw-r--r--   0        0        0    10524 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/tools/repair_tools.py
+-rw-r--r--   0        0        0     1670 2024-04-29 07:42:31.456221 ansys_geometry_core-0.5.2/src/ansys/geometry/core/typing.py
+-rw-r--r--   0        0        0     9183 1970-01-01 00:00:00.000000 ansys_geometry_core-0.5.2/PKG-INFO
```

### Comparing `ansys_geometry_core-0.5.1/LICENSE` & `ansys_geometry_core-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/README.rst` & `ansys_geometry_core-0.5.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 ^^^^^^^^^^^
 
 This code shows how to import PyAnsys Geometry and use some basic capabilities:
 
 .. code:: python
 
    from ansys.geometry.core import launch_modeler
-   from ansys.geometry.core.designer import DesignFileFormat
    from ansys.geometry.core.math import Plane, Point3D, Point2D
    from ansys.geometry.core.misc import UNITS, Distance
    from ansys.geometry.core.sketch import Sketch
 
    # Define a sketch
    origin = Point3D([0, 0, 10])
    plane = Plane(origin, direction_x=[1, 0, 0], direction_y=[0, 1, 0])
@@ -96,16 +95,16 @@
    body = design.extrude_sketch(
        name="CylinderBody", sketch=sketch, distance=Distance(80, unit=UNITS.m)
    )
 
    # Plot the body
    design.plot()
 
-   # Download the model
-   design.download(file_location="file.scdocx", format=DesignFileFormat.SCDOCX)
+   # Export the model to SCDOCX format
+   file_path = design.export_to_scdocx()
 
 For comprehensive usage information, see `Examples`_ in the `PyAnsys Geometry documentation`_.
 
 Documentation and issues
 ^^^^^^^^^^^^^^^^^^^^^^^^
 Documentation for the latest stable release of PyAnsys Geometry is hosted at `PyAnsys Geometry documentation`_.
```

### Comparing `ansys_geometry_core-0.5.1/pyproject.toml` & `ansys_geometry_core-0.5.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-geometry-core"
-version = "0.5.1"
+version = "0.5.2"
 description = "A python wrapper for Ansys Geometry service"
 readme = "README.rst"
 requires-python = ">=3.9,<4"
 license = { file = "LICENSE" }
 authors = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 maintainers = [{ name = "ANSYS, Inc.", email = "pyansys.core@ansys.com" }]
 classifiers = [
@@ -98,14 +98,15 @@
 
 [project.urls]
 Source = "https://github.com/ansys/pyansys-geometry"
 Issues = "https://github.com/ansys/pyansys-geometry/issues"
 Discussions = "https://github.com/ansys/pyansys-geometry/discussions"
 Documentation = "https://geometry.docs.pyansys.com"
 Releases = "https://github.com/ansys/pyansys-geometry/releases"
+Changelog =  "https://github.com/ansys/pyansys-geometry/blob/main/doc/source/changelog.rst"
 
 [tool.flit.module]
 name = "ansys.geometry.core"
 
 [tool.black]
 line-length = 100
```

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/__init__.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/__init__.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/backend.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/backend.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/client.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from ansys.api.dbu.v0.admin_pb2_grpc import AdminStub
 from beartype import beartype as check_input_types
 from beartype.typing import Optional, Union
 from google.protobuf.empty_pb2 import Empty
 import grpc
 from grpc._channel import _InactiveRpcError
 from grpc_health.v1 import health_pb2, health_pb2_grpc
+import semver
 
 from ansys.geometry.core.connection.backend import BackendType
 from ansys.geometry.core.connection.defaults import DEFAULT_HOST, DEFAULT_PORT, MAX_MESSAGE_LENGTH
 from ansys.geometry.core.connection.docker_instance import LocalDockerInstance
 from ansys.geometry.core.connection.product_instance import ProductInstance
 from ansys.geometry.core.logger import LOG as logger
 from ansys.geometry.core.logger import PyGeometryCustomAdapter
@@ -189,18 +190,20 @@
         self._multiple_designs_allowed = (
             False if backend_type in (BackendType.DISCOVERY, BackendType.LINUX_SERVICE) else True
         )
 
         # retrieve the backend version
         if hasattr(grpc_backend_response, "version"):
             ver = grpc_backend_response.version
-            self._backend_version = f"{ver.major_release}.{ver.minor_release}.{ver.service_pack}"
+            self._backend_version = semver.Version(
+                ver.major_release, ver.minor_release, ver.service_pack
+            )
         else:
             logger.warning("The backend version is only available after 24.1 version.")
-            self._backend_version = "24.1.0"
+            self._backend_version = semver.Version(24, 1, 0)
 
     @property
     def backend_type(self) -> BackendType:
         """
         Backend type.
 
         Options are ``Windows Service``, ``Linux Service``, ``Discovery``,
@@ -210,23 +213,22 @@
         -----
         This method might return ``None`` because determining the backend type is
         not straightforward.
         """
         return self._backend_type
 
     @property
-    def backend_version(self) -> str:
+    def backend_version(self) -> semver.Version:
         """
         Get the current backend version.
 
         Returns
         -------
-        str
-            Backend version in semantic versioning format (that is, Ansys 24R1 SP2
-            would be ``24.1.2``).
+        ~semver.Version
+            Backend version.
         """
         return self._backend_version
 
     @property
     def multiple_designs_allowed(self) -> bool:
         """
         Flag indicating whether multiple designs are allowed.
```

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/conversions.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/conversions.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/defaults.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/defaults.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/docker_instance.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/docker_instance.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/launcher.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/product_instance.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/product_instance.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/connection/validate.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/connection/validate.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/__init__.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/beam.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/beam.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/body.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/body.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/component.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/component.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/coordinate_system.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/design.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/design.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/designpoint.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/designpoint.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/edge.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/edge.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 from ansys.api.dbu.v0.dbumodels_pb2 import EntityIdentifier
 from ansys.api.geometry.v0.edges_pb2_grpc import EdgesStub
 from beartype.typing import TYPE_CHECKING, List
 from pint import Quantity
 
 from ansys.geometry.core.connection.client import GrpcClient
 from ansys.geometry.core.connection.conversions import grpc_curve_to_curve
-from ansys.geometry.core.errors import protect_grpc
+from ansys.geometry.core.errors import GeometryRuntimeError, protect_grpc
 from ansys.geometry.core.math.point import Point3D
-from ansys.geometry.core.misc.checks import ensure_design_is_active
+from ansys.geometry.core.misc.checks import ensure_design_is_active, min_backend_version
 from ansys.geometry.core.misc.measurements import DEFAULT_UNITS
 from ansys.geometry.core.shapes.curves.trimmed_curve import ReversedTrimmedCurve, TrimmedCurve
 from ansys.geometry.core.shapes.parameterization import Interval
 
 if TYPE_CHECKING:  # pragma: no cover
     from ansys.geometry.core.designer.body import Body
     from ansys.geometry.core.designer.face import Face
@@ -103,14 +103,15 @@
 
     @property
     def is_reversed(self) -> bool:
         """Flag indicating if the edge is reversed."""
         return self._is_reversed
 
     @property
+    @min_backend_version(24, 2, 0)
     def shape(self) -> TrimmedCurve:
         """
         Underlying trimmed curve of the edge.
 
         If the edge is reversed, its shape is the ``ReversedTrimmedCurve`` type, which swaps the
         start and end points of the curve and handles parameters to allow evaluation as if the
         curve is not reversed.
@@ -138,15 +139,21 @@
         return self._shape
 
     @property
     @protect_grpc
     @ensure_design_is_active
     def length(self) -> Quantity:
         """Calculated length of the edge."""
-        return self.shape.length
+        try:
+            return self.shape.length
+        except GeometryRuntimeError:  # pragma: no cover
+            # Only for versions earlier than 24.2.0 (before the introduction of the shape property)
+            self._grpc_client.log.debug("Requesting edge length from server.")
+            length_response = self._edges_stub.GetLength(self._grpc_id)
+            return Quantity(length_response.length, DEFAULT_UNITS.SERVER_LENGTH)
 
     @property
     def curve_type(self) -> CurveType:
         """Curve type of the edge."""
         return self._curve_type
 
     @property
```

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/face.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/face.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,27 +21,31 @@
 # SOFTWARE.
 """Module for managing a face."""
 
 from enum import Enum, unique
 
 from ansys.api.dbu.v0.dbumodels_pb2 import EntityIdentifier
 from ansys.api.geometry.v0.edges_pb2_grpc import EdgesStub
-from ansys.api.geometry.v0.faces_pb2 import CreateIsoParamCurvesRequest
+from ansys.api.geometry.v0.faces_pb2 import (
+    CreateIsoParamCurvesRequest,
+    EvaluateRequest,
+    GetNormalRequest,
+)
 from ansys.api.geometry.v0.faces_pb2_grpc import FacesStub
 from ansys.api.geometry.v0.models_pb2 import Edge as GRPCEdge
 from beartype.typing import TYPE_CHECKING, List
 from pint import Quantity
 
 from ansys.geometry.core.connection.client import GrpcClient
 from ansys.geometry.core.connection.conversions import grpc_curve_to_curve, grpc_surface_to_surface
 from ansys.geometry.core.designer.edge import Edge
-from ansys.geometry.core.errors import protect_grpc
+from ansys.geometry.core.errors import GeometryRuntimeError, protect_grpc
 from ansys.geometry.core.math.point import Point3D
 from ansys.geometry.core.math.vector import UnitVector3D
-from ansys.geometry.core.misc.checks import ensure_design_is_active
+from ansys.geometry.core.misc.checks import ensure_design_is_active, min_backend_version
 from ansys.geometry.core.misc.measurements import DEFAULT_UNITS
 from ansys.geometry.core.shapes.box_uv import BoxUV
 from ansys.geometry.core.shapes.curves.trimmed_curve import TrimmedCurve
 from ansys.geometry.core.shapes.parameterization import Interval
 from ansys.geometry.core.shapes.surfaces.trimmed_surface import (
     ReversedTrimmedSurface,
     TrimmedSurface,
@@ -192,14 +196,15 @@
 
     @property
     def body(self) -> "Body":
         """Body that the face belongs to."""
         return self._body
 
     @property
+    @min_backend_version(24, 2, 0)
     def shape(self) -> TrimmedSurface:
         """
         Underlying trimmed surface of the face.
 
         If the face is reversed, its shape is a ``ReversedTrimmedSurface`` type, which handles the
         direction of the normal vector to ensure it is always facing outward.
         """
@@ -301,15 +306,21 @@
         Returns
         -------
         UnitVector3D
             :class:`UnitVector3D` object evaluated at the given U and V coordinates.
             This :class:`UnitVector3D` object is perpendicular to the surface at the
             given UV coordinates.
         """
-        return self.shape.normal(u, v)
+        try:
+            return self.shape.normal(u, v)
+        except GeometryRuntimeError:  # pragma: no cover
+            # Only for versions earlier than 24.2.0 (before the introduction of the shape property)
+            self._grpc_client.log.debug(f"Requesting face normal from server with (u,v)=({u},{v}).")
+            response = self._faces_stub.GetNormal(GetNormalRequest(id=self.id, u=u, v=v)).direction
+            return UnitVector3D([response.x, response.y, response.z])
 
     @protect_grpc
     def point(self, u: float = 0.5, v: float = 0.5) -> Point3D:
         """
         Get a point of the face evaluated at certain proportional UV coordinates.
 
         Notes
@@ -329,15 +340,21 @@
 
         Returns
         -------
         Point3D
             :class:`Point3D`
             object evaluated at the given UV coordinates.
         """
-        return self.shape.evaluate_proportion(u, v).position
+        try:
+            return self.shape.evaluate_proportion(u, v).position
+        except GeometryRuntimeError:  # pragma: no cover
+            # Only for versions earlier than 24.2.0 (before the introduction of the shape property)
+            self._grpc_client.log.debug(f"Requesting face point from server with (u,v)=({u},{v}).")
+            response = self._faces_stub.Evaluate(EvaluateRequest(id=self.id, u=u, v=v)).point
+            return Point3D([response.x, response.y, response.z], DEFAULT_UNITS.SERVER_LENGTH)
 
     def __grpc_edges_to_edges(self, edges_grpc: List[GRPCEdge]) -> List[Edge]:
         """
         Transform a list of gRPC edge messages into actual ``Edge`` objects.
 
         Parameters
         ----------
```

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/part.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/part.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/designer/selection.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/designer/selection.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/errors.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/logger.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/materials/__init__.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/materials/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/materials/material.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/materials/material.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/materials/property.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/materials/property.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/__init__.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/bbox.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/bbox.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/constants.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/frame.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/frame.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/matrix.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/matrix.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/plane.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/plane.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/point.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/point.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/math/vector.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/math/vector.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/__init__.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/accuracy.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/misc/accuracy.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/auxiliary.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/misc/auxiliary.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/checks.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/misc/checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -327,27 +327,27 @@
     """
     # Lazy import to avoid circular imports
     from ansys.geometry.core.errors import GeometryRuntimeError
     from ansys.geometry.core.logger import LOG as logger
 
     def backend_version_decorator(method):
         def wrapper(self, *args, **kwargs):
-            method_version = f"{major}.{minor}.{service_pack}"
+            method_version = semver.Version(major, minor, service_pack)
             if hasattr(self, "_grpc_client"):
                 if self._grpc_client is None:
                     raise GeometryRuntimeError(
                         "The client is not available. You must initialize the client first."
                     )
                 elif self._grpc_client.backend_version is not None:
-                    comp = semver.compare(method_version, self._grpc_client.backend_version)
+                    comp = method_version.compare(self._grpc_client.backend_version)
                     # if comp is 1, method version is higher than backend version.
                     if comp == 1:
 
                         # Check if the version is "0.0.0" (i.e., the version is not available)
-                        if self._grpc_client.backend_version == "0.0.0":
+                        if str(self._grpc_client.backend_version) == "0.0.0":
                             raise GeometryRuntimeError(
                                 f"The method '{method.__name__}' requires a minimum Ansys release version of "  # noqa: E501
                                 + f"{method_version}, but the current version used is 24.1.0 or lower."  # noqa: E501
                             )
                         else:
                             raise GeometryRuntimeError(
                                 f"The method '{method.__name__}' requires a minimum Ansys release version of "  # noqa: E501
```

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/measurements.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/misc/measurements.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/options.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/misc/options.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/misc/units.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/misc/units.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/modeler.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/modeler.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/__init__.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/plotter.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/plotter_helper.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/plotter_helper.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/plotting_types.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/plotting_types.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/trame_gui.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/trame_gui.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/__init__.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/designpoint.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/downarrow.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/_images/isometric.png` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/_images/isometric.png`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/button.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/button.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/displace_arrows.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/displace_arrows.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/measure.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/measure.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/ruler.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/ruler.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/show_design_point.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/show_design_point.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/view_button.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/view_button.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/plotting/widgets/widget.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/plotting/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/__init__.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/box_uv.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/box_uv.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/__init__.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/curves/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/circle.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/curves/circle.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/curve.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/curves/curve.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/curve_evaluation.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/curves/curve_evaluation.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/ellipse.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/curves/ellipse.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/line.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/curves/line.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/curves/trimmed_curve.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/curves/trimmed_curve.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/parameterization.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/parameterization.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/__init__.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/cone.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/cone.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/cylinder.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/cylinder.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/plane.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/plane.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/sphere.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/sphere.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/surface.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/surface.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/surface_evaluation.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/torus.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/torus.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/shapes/surfaces/trimmed_surface.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/__init__.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/arc.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/arc.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/box.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/box.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/circle.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/circle.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/edge.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/edge.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/ellipse.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/ellipse.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/face.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/face.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/gears.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/gears.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/polygon.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/polygon.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/segment.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/segment.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/sketch.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/sketch.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/slot.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/slot.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/trapezoid.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/trapezoid.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/sketch/triangle.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/sketch/triangle.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/__init__.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/measurement_tools.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/tools/measurement_tools.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/problem_areas.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/tools/problem_areas.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/repair_tool_message.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/tools/repair_tool_message.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/tools/repair_tools.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/tools/repair_tools.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/src/ansys/geometry/core/typing.py` & `ansys_geometry_core-0.5.2/src/ansys/geometry/core/typing.py`

 * *Files identical despite different names*

### Comparing `ansys_geometry_core-0.5.1/PKG-INFO` & `ansys_geometry_core-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-geometry-core
-Version: 0.5.1
+Version: 0.5.2
 Summary: A python wrapper for Ansys Geometry service
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -71,14 +71,15 @@
 Requires-Dist: semver==3.0.2 ; extra == "tests"
 Requires-Dist: six==1.16.0 ; extra == "tests"
 Requires-Dist: vtk==9.3.0 ; extra == "tests"
 Requires-Dist: pytest==8.1.1 ; extra == "tests-minimal"
 Requires-Dist: pytest-cov==5.0.0 ; extra == "tests-minimal"
 Requires-Dist: pytest-pyvista==0.1.9 ; extra == "tests-minimal"
 Requires-Dist: pytest-xvfb==3.0.0 ; extra == "tests-minimal"
+Project-URL: Changelog, https://github.com/ansys/pyansys-geometry/blob/main/doc/source/changelog.rst
 Project-URL: Discussions, https://github.com/ansys/pyansys-geometry/discussions
 Project-URL: Documentation, https://geometry.docs.pyansys.com
 Project-URL: Issues, https://github.com/ansys/pyansys-geometry/issues
 Project-URL: Releases, https://github.com/ansys/pyansys-geometry/releases
 Project-URL: Source, https://github.com/ansys/pyansys-geometry
 Provides-Extra: all
 Provides-Extra: doc
@@ -155,15 +156,14 @@
 ^^^^^^^^^^^
 
 This code shows how to import PyAnsys Geometry and use some basic capabilities:
 
 .. code:: python
 
    from ansys.geometry.core import launch_modeler
-   from ansys.geometry.core.designer import DesignFileFormat
    from ansys.geometry.core.math import Plane, Point3D, Point2D
    from ansys.geometry.core.misc import UNITS, Distance
    from ansys.geometry.core.sketch import Sketch
 
    # Define a sketch
    origin = Point3D([0, 0, 10])
    plane = Plane(origin, direction_x=[1, 0, 0], direction_y=[0, 1, 0])
@@ -183,16 +183,16 @@
    body = design.extrude_sketch(
        name="CylinderBody", sketch=sketch, distance=Distance(80, unit=UNITS.m)
    )
 
    # Plot the body
    design.plot()
 
-   # Download the model
-   design.download(file_location="file.scdocx", format=DesignFileFormat.SCDOCX)
+   # Export the model to SCDOCX format
+   file_path = design.export_to_scdocx()
 
 For comprehensive usage information, see `Examples`_ in the `PyAnsys Geometry documentation`_.
 
 Documentation and issues
 ^^^^^^^^^^^^^^^^^^^^^^^^
 Documentation for the latest stable release of PyAnsys Geometry is hosted at `PyAnsys Geometry documentation`_.
```

