# Comparing `tmp/feffery_leaflet_components-0.1.0rc3.tar.gz` & `tmp/feffery_leaflet_components-0.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feffery_leaflet_components-0.1.0rc3.tar", last modified: Thu Mar 28 14:30:48 2024, max compression
+gzip compressed data, was "feffery_leaflet_components-0.1.0rc4.tar", last modified: Mon Apr 29 02:37:48 2024, max compression
```

## Comparing `feffery_leaflet_components-0.1.0rc3.tar` & `feffery_leaflet_components-0.1.0rc4.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 14:30:48.462844 feffery_leaflet_components-0.1.0rc3/
--rw-rw-rw-   0        0        0     1085 2024-01-29 03:10:24.000000 feffery_leaflet_components-0.1.0rc3/LICENSE
--rw-rw-rw-   0        0        0      504 2024-01-29 03:10:24.000000 feffery_leaflet_components-0.1.0rc3/MANIFEST.in
--rw-rw-rw-   0        0        0      302 2024-03-28 14:30:48.461833 feffery_leaflet_components-0.1.0rc3/PKG-INFO
--rw-rw-rw-   0        0        0     1534 2024-01-29 03:10:24.000000 feffery_leaflet_components-0.1.0rc3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 14:30:48.451931 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/
--rw-rw-rw-   0        0        0     2639 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/EsriTiledMapLayer.py
--rw-rw-rw-   0        0        0     1630 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/Fragment.py
--rw-rw-rw-   0        0        0     2577 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletAntPath.py
--rw-rw-rw-   0        0        0     2546 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletCircle.py
--rw-rw-rw-   0        0        0     2563 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletCircleMarker.py
--rw-rw-rw-   0        0        0     1674 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletDomWrapper.py
--rw-rw-rw-   0        0        0     2232 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletExport.py
--rw-rw-rw-   0        0        0     2065 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletFeatureGroup.py
--rw-rw-rw-   0        0        0     3295 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletFlowLayer.py
--rw-rw-rw-   0        0        0     1767 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletFullscreenControl.py
--rw-rw-rw-   0        0        0     6410 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletGeoJSON.py
--rw-rw-rw-   0        0        0     2080 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletHeatMap.py
--rw-rw-rw-   0        0        0     1777 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletLayerGroup.py
--rw-rw-rw-   0        0        0     6615 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletMap.py
--rw-rw-rw-   0        0        0     2455 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletMapAction.py
--rw-rw-rw-   0        0        0     2270 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletMapListener.py
--rw-rw-rw-   0        0        0     1670 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletMapProvider.py
--rw-rw-rw-   0        0        0     1803 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletMapSync.py
--rw-rw-rw-   0        0        0     3384 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletMarker.py
--rw-rw-rw-   0        0        0     3410 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletMiniMap.py
--rw-rw-rw-   0        0        0     2689 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletPolygon.py
--rw-rw-rw-   0        0        0     3132 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletPolyline.py
--rw-rw-rw-   0        0        0     2109 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletPopup.py
--rw-rw-rw-   0        0        0     2538 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletRectangle.py
--rw-rw-rw-   0        0        0     2061 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletStaticHeatMap.py
--rw-rw-rw-   0        0        0     4586 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletSuperCluster.py
--rw-rw-rw-   0        0        0     2041 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletTileLayer.py
--rw-rw-rw-   0        0        0     2771 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletTileSelect.py
--rw-rw-rw-   0        0        0     2229 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletTooltip.py
--rw-rw-rw-   0        0        0     2667 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletVectorTile.py
--rw-rw-rw-   0        0        0     1660 2024-03-05 06:41:33.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/MapProvider.py
--rw-rw-rw-   0        0        0     2614 2024-01-29 03:10:24.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/__init__.py
--rw-rw-rw-   0        0        0     2169 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/_imports_.py
--rw-rw-rw-   0        0        0     2334 2024-03-05 06:54:56.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/alias.py
--rw-rw-rw-   0        0        0     7819 2024-01-29 03:10:24.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/coloring_utils.py
--rw-rw-rw-   0        0        0  1180562 2024-03-28 14:30:36.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/feffery_leaflet_components.min.js
--rw-rw-rw-   0        0        0      110 2024-03-28 14:30:36.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/feffery_leaflet_components.min.js.map
--rw-rw-rw-   0        0        0    14910 2024-01-29 03:10:24.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/geometry_utils.py
--rw-rw-rw-   0        0        0   128265 2024-03-28 14:30:40.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/metadata.json
--rw-rw-rw-   0        0        0     3279 2024-03-28 14:30:38.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/package-info.json
-drwxrwxrwx   0        0        0        0 2024-03-28 14:30:48.460530 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components.egg-info/
--rw-rw-rw-   0        0        0      302 2024-03-28 14:30:48.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2157 2024-03-28 14:30:48.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 14:30:48.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-03-28 14:30:48.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-03-28 14:30:48.000000 feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3279 2024-03-28 14:29:18.000000 feffery_leaflet_components-0.1.0rc3/package.json
--rw-rw-rw-   0        0        0       42 2024-03-28 14:30:48.462844 feffery_leaflet_components-0.1.0rc3/setup.cfg
--rw-rw-rw-   0        0        0      583 2024-01-29 03:10:24.000000 feffery_leaflet_components-0.1.0rc3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 02:37:48.460564 feffery_leaflet_components-0.1.0rc4/
+-rw-rw-rw-   0        0        0     1085 2024-01-29 03:10:24.000000 feffery_leaflet_components-0.1.0rc4/LICENSE
+-rw-rw-rw-   0        0        0      504 2024-01-29 03:10:24.000000 feffery_leaflet_components-0.1.0rc4/MANIFEST.in
+-rw-rw-rw-   0        0        0      302 2024-04-29 02:37:48.459088 feffery_leaflet_components-0.1.0rc4/PKG-INFO
+-rw-rw-rw-   0        0        0     1534 2024-01-29 03:10:24.000000 feffery_leaflet_components-0.1.0rc4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 02:37:48.448513 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/
+-rw-rw-rw-   0        0        0     2669 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/EsriTiledMapLayer.py
+-rw-rw-rw-   0        0        0     1630 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/Fragment.py
+-rw-rw-rw-   0        0        0     2577 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletAntPath.py
+-rw-rw-rw-   0        0        0     2546 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletCircle.py
+-rw-rw-rw-   0        0        0     2563 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletCircleMarker.py
+-rw-rw-rw-   0        0        0     1674 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletDomWrapper.py
+-rw-rw-rw-   0        0        0     2232 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletExport.py
+-rw-rw-rw-   0        0        0     2065 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletFeatureGroup.py
+-rw-rw-rw-   0        0        0     3295 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletFlowLayer.py
+-rw-rw-rw-   0        0        0     1767 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletFullscreenControl.py
+-rw-rw-rw-   0        0        0     6410 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletGeoJSON.py
+-rw-rw-rw-   0        0        0     2080 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletHeatMap.py
+-rw-rw-rw-   0        0        0     2745 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletImageOverlay.py
+-rw-rw-rw-   0        0        0     1777 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletLayerGroup.py
+-rw-rw-rw-   0        0        0     6615 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletMap.py
+-rw-rw-rw-   0        0        0     2455 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletMapAction.py
+-rw-rw-rw-   0        0        0     2270 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletMapListener.py
+-rw-rw-rw-   0        0        0     1670 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletMapProvider.py
+-rw-rw-rw-   0        0        0     2020 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletMapSync.py
+-rw-rw-rw-   0        0        0     3384 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletMarker.py
+-rw-rw-rw-   0        0        0     3410 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletMiniMap.py
+-rw-rw-rw-   0        0        0     2689 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletPolygon.py
+-rw-rw-rw-   0        0        0     3132 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletPolyline.py
+-rw-rw-rw-   0        0        0     2109 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletPopup.py
+-rw-rw-rw-   0        0        0     2538 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletRectangle.py
+-rw-rw-rw-   0        0        0     2061 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletStaticHeatMap.py
+-rw-rw-rw-   0        0        0     4586 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletSuperCluster.py
+-rw-rw-rw-   0        0        0     2041 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletTileLayer.py
+-rw-rw-rw-   0        0        0     2771 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletTileSelect.py
+-rw-rw-rw-   0        0        0     2229 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletTooltip.py
+-rw-rw-rw-   0        0        0     2667 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletVectorTile.py
+-rw-rw-rw-   0        0        0     1660 2024-03-05 06:41:33.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/MapProvider.py
+-rw-rw-rw-   0        0        0     2614 2024-01-29 03:10:24.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/__init__.py
+-rw-rw-rw-   0        0        0     2251 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/_imports_.py
+-rw-rw-rw-   0        0        0     2425 2024-04-11 03:16:33.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/alias.py
+-rw-rw-rw-   0        0        0     7819 2024-01-29 03:10:24.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/coloring_utils.py
+-rw-rw-rw-   0        0        0  1183951 2024-04-29 02:37:40.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/feffery_leaflet_components.min.js
+-rw-rw-rw-   0        0        0      110 2024-04-29 02:37:40.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/feffery_leaflet_components.min.js.map
+-rw-rw-rw-   0        0        0    14910 2024-01-29 03:10:24.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/geometry_utils.py
+-rw-rw-rw-   0        0        0   132430 2024-04-29 02:37:43.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/metadata.json
+-rw-rw-rw-   0        0        0     3317 2024-04-29 02:37:41.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/package-info.json
+drwxrwxrwx   0        0        0        0 2024-04-29 02:37:48.459088 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components.egg-info/
+-rw-rw-rw-   0        0        0      302 2024-04-29 02:37:48.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2207 2024-04-29 02:37:48.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 02:37:48.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-29 02:37:48.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-29 02:37:48.000000 feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3317 2024-04-29 02:34:54.000000 feffery_leaflet_components-0.1.0rc4/package.json
+-rw-rw-rw-   0        0        0       42 2024-04-29 02:37:48.462061 feffery_leaflet_components-0.1.0rc4/setup.cfg
+-rw-rw-rw-   0        0        0      583 2024-01-29 03:10:24.000000 feffery_leaflet_components-0.1.0rc4/setup.py
```

### Comparing `feffery_leaflet_components-0.1.0rc3/LICENSE` & `feffery_leaflet_components-0.1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/README.md` & `feffery_leaflet_components-0.1.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/EsriTiledMapLayer.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/EsriTiledMapLayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # AUTO GENERATED FILE - DO NOT EDIT
 
 from dash.development.base_component import Component, _explicitize_args
 
 
 class EsriTiledMapLayer(Component):
     """An EsriTiledMapLayer component.
-
+ESRI tiledMapLayer图层组件
 
 Keyword arguments:
 
 - id (string; optional)
 
 - debug (boolean; default False):
     是否开启debug模式  默认：False.
```

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/Fragment.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/Fragment.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletAntPath.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletAntPath.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletCircle.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletCircle.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletCircleMarker.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletCircleMarker.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletDomWrapper.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletDomWrapper.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletExport.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletExport.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletFeatureGroup.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletFeatureGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletFlowLayer.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletFlowLayer.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletFullscreenControl.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletFullscreenControl.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletGeoJSON.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletGeoJSON.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletHeatMap.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletHeatMap.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletLayerGroup.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletLayerGroup.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletMap.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletMap.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletMapAction.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletMapAction.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletMapListener.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletMapListener.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletMapProvider.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletMapProvider.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletMapSync.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletMapSync.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,24 +25,27 @@
     - component_name (string; optional):
         Holds the name of the component that is loading.
 
     - is_loading (boolean; optional):
         Determines if the component is loading or not.
 
     - prop_name (string; optional):
-        Holds which property is loading."""
+        Holds which property is loading.
+
+- syncStrategy (a value equal to: 'all', 'center'; default 'all'):
+    同步行为策略，可选项有`'all'`、`'center'`  默认值：`'all'`."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_leaflet_components'
     _type = 'LeafletMapSync'
     @_explicitize_args
-    def __init__(self, id=Component.REQUIRED, key=Component.UNDEFINED, groupId=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'groupId', 'key', 'loading_state']
+    def __init__(self, id=Component.REQUIRED, key=Component.UNDEFINED, groupId=Component.UNDEFINED, syncStrategy=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'groupId', 'key', 'loading_state', 'syncStrategy']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'groupId', 'key', 'loading_state']
+        self.available_properties = ['id', 'groupId', 'key', 'loading_state', 'syncStrategy']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         for k in ['id']:
```

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletMarker.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletMarker.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletMiniMap.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletMiniMap.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletPolygon.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletPolygon.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletPolyline.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletPolyline.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletPopup.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletPopup.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletRectangle.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletRectangle.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletStaticHeatMap.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletStaticHeatMap.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletSuperCluster.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletSuperCluster.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletTileLayer.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletTileLayer.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletTileSelect.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletTileSelect.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletTooltip.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletTooltip.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/LeafletVectorTile.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/LeafletVectorTile.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/MapProvider.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/MapProvider.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/__init__.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/__init__.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/_imports_.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/_imports_.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .LeafletDomWrapper import LeafletDomWrapper
 from .LeafletExport import LeafletExport
 from .LeafletFeatureGroup import LeafletFeatureGroup
 from .LeafletFlowLayer import LeafletFlowLayer
 from .LeafletFullscreenControl import LeafletFullscreenControl
 from .LeafletGeoJSON import LeafletGeoJSON
 from .LeafletHeatMap import LeafletHeatMap
+from .LeafletImageOverlay import LeafletImageOverlay
 from .LeafletLayerGroup import LeafletLayerGroup
 from .LeafletMap import LeafletMap
 from .LeafletMapAction import LeafletMapAction
 from .LeafletMapListener import LeafletMapListener
 from .LeafletMapProvider import LeafletMapProvider
 from .LeafletMapSync import LeafletMapSync
 from .LeafletMarker import LeafletMarker
@@ -38,14 +39,15 @@
     "LeafletDomWrapper",
     "LeafletExport",
     "LeafletFeatureGroup",
     "LeafletFlowLayer",
     "LeafletFullscreenControl",
     "LeafletGeoJSON",
     "LeafletHeatMap",
+    "LeafletImageOverlay",
     "LeafletLayerGroup",
     "LeafletMap",
     "LeafletMapAction",
     "LeafletMapListener",
     "LeafletMapProvider",
     "LeafletMapSync",
     "LeafletMarker",
```

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/alias.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/alias.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .LeafletDomWrapper import LeafletDomWrapper as DomWrapper
 from .LeafletExport import LeafletExport as Export
 from .LeafletFeatureGroup import LeafletFeatureGroup as FeatureGroup
 from .LeafletFlowLayer import LeafletFlowLayer as FlowLayer
 from .LeafletFullscreenControl import LeafletFullscreenControl as FullscreenControl
 from .LeafletGeoJSON import LeafletGeoJSON as GeoJSON
 from .LeafletHeatMap import LeafletHeatMap as HeatMap
+from .LeafletImageOverlay import LeafletImageOverlay as ImageOverlay
 from .LeafletLayerGroup import LeafletLayerGroup as LayerGroup
 from .LeafletMap import LeafletMap as Map
 from .LeafletMapAction import LeafletMapAction as MapAction
 from .LeafletMapListener import LeafletMapListener as MapListener
 from .LeafletMapProvider import LeafletMapProvider as MapProvider
 from .LeafletMapSync import LeafletMapSync as MapSync
 from .LeafletMarker import LeafletMarker as Marker
@@ -38,14 +39,15 @@
     "DomWrapper",
     "Export",
     "FeatureGroup",
     "FlowLayer",
     "FullscreenControl",
     "GeoJSON",
     "HeatMap",
+    "ImageOverlay",
     "LayerGroup",
     "Map",
     "MapAction",
     "MapListener",
     "MapProvider",
     "MapSync",
     "Marker",
```

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/coloring_utils.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/coloring_utils.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/feffery_leaflet_components.min.js` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/feffery_leaflet_components.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -64,15 +64,15 @@
             var e = function(t) {
                     return /\/_dash-component-suites\//.test(t.src)
                 }(r()),
                 n = o(t);
             if (!e) return n;
             var i = n.split("/"),
                 a = i.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_1_0-rc3m1711636227"), i.splice(-1, 1, a.join(".")), i.join("/")
+            return a.splice(1, 0, "v0_1_0-rc4m1714358248"), i.splice(-1, 1, a.join(".")), i.join("/")
         }
     }
     return n(n.s = 80)
 }([function(t, e) {
     t.exports = window.PropTypes
 }, function(t, e) {
     t.exports = window.React
@@ -738,23 +738,23 @@
             _transform: function(t, e) {
                 return e = e || 1, t.x = e * (this._a * t.x + this._b), t.y = e * (this._c * t.y + this._d), t
             },
             untransform: function(t, e) {
                 return e = e || 1, new I((t.x / e - this._b) / this._a, (t.y / e - this._d) / this._c)
             }
         };
-        var Y = e({}, Z, {
+        var q = e({}, Z, {
                 code: "EPSG:3857",
                 projection: W,
                 transformation: function() {
                     var t = .5 / (Math.PI * W.R);
                     return H(t, .5, -t, .5)
                 }()
             }),
-            q = e({}, Y, {
+            Y = e({}, q, {
                 code: "EPSG:900913"
             });
 
         function Q(t) {
             return document.createElementNS("http://www.w3.org/2000/svg", t)
         }
 
@@ -900,15 +900,15 @@
 
         function Ht(t, e) {
             if (e.pointerType !== (e.MSPOINTER_TYPE_MOUSE || "mouse")) {
                 for (var n in e.touches = [], Ut) e.touches.push(Ut[n]);
                 e.changedTouches = [e], t(e)
             }
         }
-        var Yt, qt, Qt, Kt, Jt, Xt = de(["transform", "webkitTransform", "OTransform", "MozTransform", "msTransform"]),
+        var qt, Yt, Qt, Kt, Jt, Xt = de(["transform", "webkitTransform", "OTransform", "MozTransform", "msTransform"]),
             $t = de(["webkitTransition", "transition", "OTransition", "MozTransition", "msTransition"]),
             te = "webkitTransition" === $t || "OTransition" === $t ? $t + "End" : "transitionend";
 
         function ee(t) {
             return "string" == typeof t ? document.getElementById(t) : t
         }
 
@@ -999,27 +999,27 @@
         function ge(t, e) {
             t._leaflet_pos = e, jt.any3d ? me(t, e) : (t.style.left = e.x + "px", t.style.top = e.y + "px")
         }
 
         function ye(t) {
             return t._leaflet_pos || new I(0, 0)
         }
-        if ("onselectstart" in document) Yt = function() {
+        if ("onselectstart" in document) qt = function() {
             ke(window, "selectstart", ze)
-        }, qt = function() {
+        }, Yt = function() {
             Se(window, "selectstart", ze)
         };
         else {
             var _e = de(["userSelect", "WebkitUserSelect", "OUserSelect", "MozUserSelect", "msUserSelect"]);
-            Yt = function() {
+            qt = function() {
                 if (_e) {
                     var t = document.documentElement.style;
                     Qt = t[_e], t[_e] = "none"
                 }
-            }, qt = function() {
+            }, Yt = function() {
                 _e && (document.documentElement.style[_e] = Qt, Qt = void 0)
             }
         }
 
         function ve() {
             ke(window, "dragstart", ze)
         }
@@ -1071,18 +1071,18 @@
             getClass: fe,
             setOpacity: pe,
             testProp: de,
             setTransform: me,
             setPosition: ge,
             getPosition: ye,
             get disableTextSelection() {
-                return Yt
+                return qt
             },
             get enableTextSelection() {
-                return qt
+                return Yt
             },
             disableImageDrag: ve,
             enableImageDrag: be,
             preventOutline: Me,
             restoreOutline: we,
             getSizedParentNode: xe,
             getScale: Le
@@ -1261,15 +1261,15 @@
                 },
                 _easeOut: function(t) {
                     return 1 - Math.pow(1 - t, this._easeOutPower)
                 }
             }),
             Ve = E.extend({
                 options: {
-                    crs: Y,
+                    crs: q,
                     center: void 0,
                     zoom: void 0,
                     minZoom: void 0,
                     maxZoom: void 0,
                     layers: [],
                     maxBounds: void 0,
                     renderer: void 0,
@@ -1906,15 +1906,15 @@
                 remove: function() {
                     return this._map ? (re(this._container), this.onRemove && this.onRemove(this._map), this._map.off("unload", this.remove, this), this._map = null, this) : this
                 },
                 _refocusOnMap: function(t) {
                     this._map && t && t.screenX > 0 && t.screenY > 0 && this._map.getContainer().focus()
                 }
             }),
-            Ye = function(t) {
+            qe = function(t) {
                 return new He(t)
             };
         Ve.include({
             addControl: function(t) {
                 return t.addTo(this), this
             },
             removeControl: function(t) {
@@ -1932,15 +1932,15 @@
                 i("top", "left"), i("top", "right"), i("bottom", "left"), i("bottom", "right")
             },
             _clearControlPos: function() {
                 for (var t in this._controlCorners) re(this._controlCorners[t]);
                 re(this._controlContainer), delete this._controlCorners, delete this._controlContainer
             }
         });
-        var qe = He.extend({
+        var Ye = He.extend({
                 options: {
                     collapsed: !0,
                     position: "topright",
                     autoZIndex: !0,
                     hideSingleBase: !1,
                     sortLayers: !1,
                     sortFunction: function(t, e, n, i) {
@@ -2196,21 +2196,21 @@
                     }
                 }
             });
         Ve.mergeOptions({
             attributionControl: !0
         }), Ve.addInitHook((function() {
             this.options.attributionControl && (new Je).addTo(this)
-        })), He.Layers = qe, He.Zoom = Qe, He.Scale = Ke, He.Attribution = Je, Ye.layers = function(t, e, n) {
-            return new qe(t, e, n)
-        }, Ye.zoom = function(t) {
+        })), He.Layers = Ye, He.Zoom = Qe, He.Scale = Ke, He.Attribution = Je, qe.layers = function(t, e, n) {
+            return new Ye(t, e, n)
+        }, qe.zoom = function(t) {
             return new Qe(t)
-        }, Ye.scale = function(t) {
+        }, qe.scale = function(t) {
             return new Ke(t)
-        }, Ye.attribution = function(t) {
+        }, qe.attribution = function(t) {
             return new Je(t)
         };
         var Xe = C.extend({
             initialize: function(t) {
                 this._map = t
             },
             enable: function() {
@@ -2242,15 +2242,15 @@
                 },
                 disable: function() {
                     this._enabled && (en._dragging === this && this.finishDrag(!0), Se(this._dragStartTarget, tn, this._onDown, this), this._enabled = !1, this._moved = !1)
                 },
                 _onDown: function(t) {
                     if (this._enabled && (this._moved = !1, !le(this._element, "leaflet-zoom-anim")))
                         if (t.touches && 1 !== t.touches.length) en._dragging === this && this.finishDrag();
-                        else if (!(en._dragging || t.shiftKey || 1 !== t.which && 1 !== t.button && !t.touches || (en._dragging = this, this._preventOutline && Me(this._element), ve(), Yt(), this._moving))) {
+                        else if (!(en._dragging || t.shiftKey || 1 !== t.which && 1 !== t.button && !t.touches || (en._dragging = this, this._preventOutline && Me(this._element), ve(), qt(), this._moving))) {
                         this.fire("down");
                         var e = t.touches ? t.touches[0] : t,
                             n = xe(this._element);
                         this._startPoint = new I(e.clientX, e.clientY), this._startPos = ye(this._element), this._parentScale = Le(n);
                         var i = "mousedown" === t.type;
                         ke(document, i ? "mousemove" : "touchmove", this._onMove, this), ke(document, i ? "mouseup" : "touchend touchcancel", this._onUp, this)
                     }
@@ -2270,15 +2270,15 @@
                     };
                     this.fire("predrag", t), ge(this._element, this._newPos), this.fire("drag", t)
                 },
                 _onUp: function() {
                     this._enabled && this.finishDrag()
                 },
                 finishDrag: function(t) {
-                    he(document.body, "leaflet-dragging"), this._lastTarget && (he(this._lastTarget, "leaflet-drag-target"), this._lastTarget = null), Se(document, "mousemove touchmove", this._onMove, this), Se(document, "mouseup touchend touchcancel", this._onUp, this), be(), qt();
+                    he(document.body, "leaflet-dragging"), this._lastTarget && (he(this._lastTarget, "leaflet-drag-target"), this._lastTarget = null), Se(document, "mousemove touchmove", this._onMove, this), Se(document, "mouseup touchend touchcancel", this._onUp, this), be(), Yt();
                     var e = this._moved && this._moving;
                     this._moving = !1, en._dragging = !1, e && this.fire("dragend", {
                         noInertia: t,
                         distance: this._newPos.distanceTo(this._startPos)
                     })
                 }
             });
@@ -2489,15 +2489,15 @@
                 distance: function(t, e) {
                     var n = e.lng - t.lng,
                         i = e.lat - t.lat;
                     return Math.sqrt(n * n + i * i)
                 },
                 infinite: !0
             });
-        G.Earth = Z, G.EPSG3395 = Mn, G.EPSG3857 = Y, G.EPSG900913 = q, G.EPSG4326 = wn, G.Simple = xn;
+        G.Earth = Z, G.EPSG3395 = Mn, G.EPSG3857 = q, G.EPSG900913 = Y, G.EPSG4326 = wn, G.Simple = xn;
         var Ln = E.extend({
             options: {
                 pane: "overlayPane",
                 attribution: null,
                 bubblingMouseEvents: !0
             },
             addTo: function(t) {
@@ -3347,16 +3347,16 @@
                     type: "GeometryCollection"
                 }) : {
                     type: "FeatureCollection",
                     features: i
                 }
             }
         });
-        var Yn = Hn,
-            qn = Ln.extend({
+        var qn = Hn,
+            Yn = Ln.extend({
                 options: {
                     opacity: 1,
                     alt: "",
                     interactive: !1,
                     crossOrigin: !1,
                     errorOverlayUrl: "",
                     zIndex: 1,
@@ -3432,15 +3432,15 @@
                     var t = this.options.errorOverlayUrl;
                     t && this._url !== t && (this._url = t, this._image.src = t)
                 },
                 getCenter: function() {
                     return this._bounds.getCenter()
                 }
             }),
-            Qn = qn.extend({
+            Qn = Yn.extend({
                 options: {
                     autoplay: !0,
                     loop: !0,
                     keepAspectRatio: !0,
                     muted: !1,
                     playsInline: !0
                 },
@@ -3455,15 +3455,15 @@
                         for (var a = 0; a < this._url.length; a++) {
                             var s = ie("source");
                             s.src = this._url[a], e.appendChild(s)
                         }
                     }
                 }
             }),
-            Kn = qn.extend({
+            Kn = Yn.extend({
                 _initImage: function() {
                     var t = this._image = this._url;
                     ue(t, "leaflet-image-layer"), this._zoomAnimated && ue(t, "leaflet-zoom-animated"), this.options.className && ue(t, this.options.className), t.onselectstart = u, t.onmousemove = u
                 }
             }),
             Jn = Ln.extend({
                 options: {
@@ -4721,29 +4721,29 @@
                 this._resetStateTimeout = 0, this._moved = !1
             },
             _clearDeferredResetState: function() {
                 0 !== this._resetStateTimeout && (clearTimeout(this._resetStateTimeout), this._resetStateTimeout = 0)
             },
             _onMouseDown: function(t) {
                 if (!t.shiftKey || 1 !== t.which && 1 !== t.button) return !1;
-                this._clearDeferredResetState(), this._resetState(), Yt(), ve(), this._startPoint = this._map.mouseEventToContainerPoint(t), ke(document, {
+                this._clearDeferredResetState(), this._resetState(), qt(), ve(), this._startPoint = this._map.mouseEventToContainerPoint(t), ke(document, {
                     contextmenu: Ne,
                     mousemove: this._onMouseMove,
                     mouseup: this._onMouseUp,
                     keydown: this._onKeyDown
                 }, this)
             },
             _onMouseMove: function(t) {
                 this._moved || (this._moved = !0, this._box = ie("div", "leaflet-zoom-box", this._container), ue(this._container, "leaflet-crosshair"), this._map.fire("boxzoomstart")), this._point = this._map.mouseEventToContainerPoint(t);
                 var e = new D(this._point, this._startPoint),
                     n = e.getSize();
                 ge(this._box, e.min), this._box.style.width = n.x + "px", this._box.style.height = n.y + "px"
             },
             _finish: function() {
-                this._moved && (re(this._box), he(this._container, "leaflet-crosshair")), qt(), be(), Se(document, {
+                this._moved && (re(this._box), he(this._container, "leaflet-crosshair")), Yt(), be(), Se(document, {
                     contextmenu: Ne,
                     mousemove: this._onMouseMove,
                     mouseup: this._onMouseUp,
                     keydown: this._onKeyDown
                 }, this)
             },
             _onMouseUp: function(t) {
@@ -5085,28 +5085,28 @@
                     this._animRequest = k(s, this, !0), ze(t)
                 }
             },
             _onTouchEnd: function() {
                 this._moved && this._zooming ? (this._zooming = !1, O(this._animRequest), Se(document, "touchmove", this._onTouchMove, this), Se(document, "touchend touchcancel", this._onTouchEnd, this), this._map.options.zoomAnimation ? this._map._animateZoom(this._center, this._map._limitZoom(this._zoom), !0, this._map.options.zoomSnap) : this._map._resetView(this._center, this._map._limitZoom(this._zoom))) : this._zooming = !1
             }
         });
-        Ve.addInitHook("addHandler", "touchZoom", bi), Ve.BoxZoom = di, Ve.DoubleClickZoom = mi, Ve.Drag = gi, Ve.Keyboard = yi, Ve.ScrollWheelZoom = _i, Ve.TapHold = vi, Ve.TouchZoom = bi, t.Bounds = D, t.Browser = jt, t.CRS = G, t.Canvas = ai, t.Circle = jn, t.CircleMarker = In, t.Class = C, t.Control = He, t.DivIcon = ti, t.DivOverlay = Jn, t.DomEvent = Ze, t.DomUtil = Ae, t.Draggable = en, t.Evented = E, t.FeatureGroup = kn, t.GeoJSON = zn, t.GridLayer = ei, t.Handler = Xe, t.Icon = On, t.ImageOverlay = qn, t.LatLng = R, t.LatLngBounds = N, t.Layer = Ln, t.LayerGroup = An, t.LineUtil = yn, t.Map = Ve, t.Marker = Pn, t.Mixin = $e, t.Path = En, t.Point = I, t.PolyUtil = sn, t.Polygon = Dn, t.Polyline = Tn, t.Popup = Xn, t.PosAnimation = We, t.Projection = bn, t.Rectangle = pi, t.Renderer = oi, t.SVG = ci, t.SVGOverlay = Kn, t.TileLayer = ni, t.Tooltip = $n, t.Transformation = V, t.Util = S, t.VideoOverlay = Qn, t.bind = i, t.bounds = z, t.canvas = si, t.circle = function(t, e, n) {
+        Ve.addInitHook("addHandler", "touchZoom", bi), Ve.BoxZoom = di, Ve.DoubleClickZoom = mi, Ve.Drag = gi, Ve.Keyboard = yi, Ve.ScrollWheelZoom = _i, Ve.TapHold = vi, Ve.TouchZoom = bi, t.Bounds = D, t.Browser = jt, t.CRS = G, t.Canvas = ai, t.Circle = jn, t.CircleMarker = In, t.Class = C, t.Control = He, t.DivIcon = ti, t.DivOverlay = Jn, t.DomEvent = Ze, t.DomUtil = Ae, t.Draggable = en, t.Evented = E, t.FeatureGroup = kn, t.GeoJSON = zn, t.GridLayer = ei, t.Handler = Xe, t.Icon = On, t.ImageOverlay = Yn, t.LatLng = R, t.LatLngBounds = N, t.Layer = Ln, t.LayerGroup = An, t.LineUtil = yn, t.Map = Ve, t.Marker = Pn, t.Mixin = $e, t.Path = En, t.Point = I, t.PolyUtil = sn, t.Polygon = Dn, t.Polyline = Tn, t.Popup = Xn, t.PosAnimation = We, t.Projection = bn, t.Rectangle = pi, t.Renderer = oi, t.SVG = ci, t.SVGOverlay = Kn, t.TileLayer = ni, t.Tooltip = $n, t.Transformation = V, t.Util = S, t.VideoOverlay = Qn, t.bind = i, t.bounds = z, t.canvas = si, t.circle = function(t, e, n) {
             return new jn(t, e, n)
         }, t.circleMarker = function(t, e) {
             return new In(t, e)
-        }, t.control = Ye, t.divIcon = function(t) {
+        }, t.control = qe, t.divIcon = function(t) {
             return new ti(t)
         }, t.extend = e, t.featureGroup = function(t, e) {
             return new kn(t, e)
-        }, t.geoJSON = Hn, t.geoJson = Yn, t.gridLayer = function(t) {
+        }, t.geoJSON = Hn, t.geoJson = qn, t.gridLayer = function(t) {
             return new ei(t)
         }, t.icon = function(t) {
             return new On(t)
         }, t.imageOverlay = function(t, e, n) {
-            return new qn(t, e, n)
+            return new Yn(t, e, n)
         }, t.latLng = U, t.latLngBounds = B, t.layerGroup = function(t, e) {
             return new An(t, e)
         }, t.map = function(t, e) {
             return new Ve(t, e)
         }, t.marker = function(t, e) {
             return new Pn(t, e)
         }, t.point = T, t.polygon = function(t, e) {
@@ -5187,16 +5187,16 @@
                 U = RegExp(B.source),
                 F = /<%-([\s\S]+?)%>/g,
                 G = /<%([\s\S]+?)%>/g,
                 Z = /<%=([\s\S]+?)%>/g,
                 W = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
                 V = /^\w*$/,
                 H = /[^.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|$))/g,
-                Y = /[\\^$.*+?()[\]{}|]/g,
-                q = RegExp(Y.source),
+                q = /[\\^$.*+?()[\]{}|]/g,
+                Y = RegExp(q.source),
                 Q = /^\s+/,
                 K = /\s/,
                 J = /\{(?:\n\/\* \[wrapped with .+\] \*\/)?\n?/,
                 X = /\{\n\/\* \[wrapped with (.+)\] \*/,
                 $ = /,? & /,
                 tt = /[^\x00-\x2f\x3a-\x40\x5b-\x60\x7b-\x7f]+/g,
                 et = /[()=,{}\[\]\/\s]/,
@@ -5250,16 +5250,16 @@
                     "\r": "r",
                     "\u2028": "u2028",
                     "\u2029": "u2029"
                 },
                 Wt = parseFloat,
                 Vt = parseInt,
                 Ht = "object" == (void 0 === t ? "undefined" : o(t)) && t && t.Object === Object && t,
-                Yt = "object" == ("undefined" == typeof self ? "undefined" : o(self)) && self && self.Object === Object && self,
-                qt = Ht || Yt || Function("return this")(),
+                qt = "object" == ("undefined" == typeof self ? "undefined" : o(self)) && self && self.Object === Object && self,
+                Yt = Ht || qt || Function("return this")(),
                 Qt = "object" == o(e) && e && !e.nodeType && e,
                 Kt = Qt && "object" == o(i) && i && !i.nodeType && i,
                 Jt = Kt && Kt.exports === Qt,
                 Xt = Jt && Ht.process,
                 $t = function() {
                     try {
                         var t = Kt && Kt.require && Kt.require("util").types;
@@ -5704,23 +5704,23 @@
                 var e = -1,
                     n = Array(t.size);
                 return t.forEach((function(t) {
                     n[++e] = [t, t]
                 })), n
             }
 
-            function Ye(t) {
+            function qe(t) {
                 return Fe(t) ? function(t) {
                     var e = Dt.lastIndex = 0;
                     for (; Dt.test(t);) ++e;
                     return e
                 }(t) : ve(t)
             }
 
-            function qe(t) {
+            function Ye(t) {
                 return Fe(t) ? function(t) {
                     return t.match(Dt) || []
                 }(t) : function(t) {
                     return t.split("")
                 }(t)
             }
 
@@ -5732,15 +5732,15 @@
                 "&amp;": "&",
                 "&lt;": "<",
                 "&gt;": ">",
                 "&quot;": '"',
                 "&#39;": "'"
             });
             var Je = function t(e) {
-                var n, i = (e = null == e ? qt : Je.defaults(qt.Object(), e, Je.pick(qt, Rt))).Array,
+                var n, i = (e = null == e ? Yt : Je.defaults(Yt.Object(), e, Je.pick(Yt, Rt))).Array,
                     r = e.Date,
                     K = e.Error,
                     pt = e.Function,
                     dt = e.Math,
                     mt = e.Object,
                     gt = e.RegExp,
                     yt = e.String,
@@ -5751,36 +5751,36 @@
                     wt = e["__core-js_shared__"],
                     xt = bt.toString,
                     Lt = Mt.hasOwnProperty,
                     At = 0,
                     kt = (n = /[^.]+$/.exec(wt && wt.keys && wt.keys.IE_PROTO || "")) ? "Symbol(src)_1." + n : "",
                     Ot = Mt.toString,
                     St = xt.call(mt),
-                    Ct = qt._,
-                    Pt = gt("^" + xt.call(Lt).replace(Y, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
+                    Ct = Yt._,
+                    Pt = gt("^" + xt.call(Lt).replace(q, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
                     Et = Jt ? e.Buffer : void 0,
                     It = e.Symbol,
                     Dt = e.Uint8Array,
                     Nt = Et ? Et.allocUnsafe : void 0,
                     Zt = Ze(mt.getPrototypeOf, mt),
                     Ht = mt.create,
-                    Yt = Mt.propertyIsEnumerable,
+                    qt = Mt.propertyIsEnumerable,
                     Qt = vt.splice,
                     Kt = It ? It.isConcatSpreadable : void 0,
                     Xt = It ? It.iterator : void 0,
                     $t = It ? It.toStringTag : void 0,
                     ve = function() {
                         try {
                             var t = eo(mt, "defineProperty");
                             return t({}, "", {}), t
                         } catch (t) {}
                     }(),
-                    Oe = e.clearTimeout !== qt.clearTimeout && e.clearTimeout,
-                    Xe = r && r.now !== qt.Date.now && r.now,
-                    $e = e.setTimeout !== qt.setTimeout && e.setTimeout,
+                    Oe = e.clearTimeout !== Yt.clearTimeout && e.clearTimeout,
+                    Xe = r && r.now !== Yt.Date.now && r.now,
+                    $e = e.setTimeout !== Yt.setTimeout && e.setTimeout,
                     tn = dt.ceil,
                     en = dt.floor,
                     nn = mt.getOwnPropertySymbols,
                     rn = Et ? Et.isBuffer : void 0,
                     on = e.isFinite,
                     an = vt.join,
                     sn = Ze(mt.keys, mt),
@@ -5909,21 +5909,21 @@
 
                 function Hn(t, e) {
                     for (var n = t.length; n--;)
                         if (Ea(t[n][0], e)) return n;
                     return -1
                 }
 
-                function Yn(t, e, n, i) {
+                function qn(t, e, n, i) {
                     return ni(t, (function(t, r, o) {
                         e(i, t, n(t), o)
                     })), i
                 }
 
-                function qn(t, e) {
+                function Yn(t, e) {
                     return t && br(e, ws(e), t)
                 }
 
                 function Qn(t, e, n) {
                     "__proto__" == e && ve ? ve(t, e, {
                         configurable: !0,
                         enumerable: !0,
@@ -5962,15 +5962,15 @@
                         if (x == _ || x == u || T && !r) {
                             if (a = l || T ? {} : ao(t), !s) return l ? function(t, e) {
                                 return br(t, io(t), e)
                             }(t, function(t, e) {
                                 return t && br(e, xs(e), t)
                             }(a, t)) : function(t, e) {
                                 return br(t, no(t), e)
-                            }(t, qn(a, t))
+                            }(t, Yn(a, t))
                         } else {
                             if (!Gt[x]) return r ? t : {};
                             a = function(t, e, n) {
                                 var i = t.constructor;
                                 switch (e) {
                                     case L:
                                         return dr(t);
@@ -6012,18 +6012,18 @@
                         }
                     }
                     o || (o = new Rn);
                     var D = o.get(t);
                     if (D) return D;
                     o.set(t, a), Ja(t) ? t.forEach((function(i) {
                         a.add(Xn(i, e, n, i, t, o))
-                    })) : Ya(t) && t.forEach((function(i, r) {
+                    })) : qa(t) && t.forEach((function(i, r) {
                         a.set(r, Xn(i, e, n, r, t, o))
                     }));
-                    var z = p ? void 0 : (h ? l ? qr : Yr : l ? xs : ws)(t);
+                    var z = p ? void 0 : (h ? l ? Yr : qr : l ? xs : ws)(t);
                     return le(z || t, (function(i, r) {
                         z && (i = t[r = i]), Vn(a, r, Xn(i, e, n, r, t, o))
                     })), a
                 }
 
                 function $n(t, e, n) {
                     var i = n.length;
@@ -6321,17 +6321,17 @@
                                 return o || (o = new Rn), r(C, P, n, i, o)
                             }
                         }
                         if (!k) return !1;
                         return o || (o = new Rn),
                             function(t, e, n, i, r, o) {
                                 var a = 1 & n,
-                                    s = Yr(t),
+                                    s = qr(t),
                                     l = s.length,
-                                    u = Yr(e).length;
+                                    u = qr(e).length;
                                 if (l != u && !a) return !1;
                                 var h = l;
                                 for (; h--;) {
                                     var c = s[h];
                                     if (!(a ? c in e : Lt.call(e, c))) return !1
                                 }
                                 var f = o.get(t),
@@ -6387,15 +6387,15 @@
 
                 function Li(t) {
                     return !(!Va(t) || (e = t, kt && kt in e)) && (Ga(t) ? Pt : st).test(Co(t));
                     var e
                 }
 
                 function Ai(t) {
-                    return "function" == typeof t ? t : null == t ? qs : "object" == o(t) ? Da(t) ? Ei(t[0], t[1]) : Pi(t) : il(t)
+                    return "function" == typeof t ? t : null == t ? Ys : "object" == o(t) ? Da(t) ? Ei(t[0], t[1]) : Pi(t) : il(t)
                 }
 
                 function ki(t) {
                     if (!po(t)) return sn(t);
                     var e = [];
                     for (var n in mt(t)) Lt.call(t, n) && "constructor" != n && e.push(n);
                     return e
@@ -6471,15 +6471,15 @@
                 }
 
                 function Ti(t, e, n) {
                     e = e.length ? de(e, (function(t) {
                         return Da(t) ? function(e) {
                             return pi(e, 1 === t.length ? t[0] : t)
                         } : t
-                    })) : [qs];
+                    })) : [Ys];
                     var i = -1;
                     return e = de(e, Ie(Xr())),
                         function(t, e) {
                             var n = t.length;
                             for (t.sort(e); n--;) t[n] = t[n].value;
                             return t
                         }(Ci(t, (function(t, n, r) {
@@ -6551,15 +6551,15 @@
                     do {
                         e % 2 && (n += t), (e = en(e / 2)) && (t += t)
                     } while (e);
                     return n
                 }
 
                 function Ui(t, e) {
-                    return xo(yo(t, e, qs), t + "")
+                    return xo(yo(t, e, Ys), t + "")
                 }
 
                 function Fi(t) {
                     return Fn(Es(t))
                 }
 
                 function Gi(t, e) {
@@ -6579,37 +6579,37 @@
                         }
                         Vn(s, l, u), s = s[l]
                     }
                     return t
                 }
                 var Wi = bn ? function(t, e) {
                         return bn.set(t, e), t
-                    } : qs,
+                    } : Ys,
                     Vi = ve ? function(t, e) {
                         return ve(t, "toString", {
                             configurable: !0,
                             enumerable: !1,
                             value: Vs(e),
                             writable: !0
                         })
-                    } : qs;
+                    } : Ys;
 
                 function Hi(t) {
                     return ko(Es(t))
                 }
 
-                function Yi(t, e, n) {
+                function qi(t, e, n) {
                     var r = -1,
                         o = t.length;
                     e < 0 && (e = -e > o ? 0 : o + e), (n = n > o ? o : n) < 0 && (n += o), o = e > n ? 0 : n - e >>> 0, e >>>= 0;
                     for (var a = i(o); ++r < o;) a[r] = t[r + e];
                     return a
                 }
 
-                function qi(t, e) {
+                function Yi(t, e) {
                     var n;
                     return ni(t, (function(t, i, r) {
                         return !(n = e(t, i, r))
                     })), !!n
                 }
 
                 function Qi(t, e, n) {
@@ -6619,15 +6619,15 @@
                         for (; i < r;) {
                             var o = i + r >>> 1,
                                 a = t[o];
                             null !== a && !$a(a) && (n ? a <= e : a < e) ? i = o + 1 : r = o
                         }
                         return r
                     }
-                    return Ki(t, e, qs, n)
+                    return Ki(t, e, Ys, n)
                 }
 
                 function Ki(t, e, n, i) {
                     var r = 0,
                         o = null == t ? 0 : t.length;
                     if (0 === o) return 0;
                     for (var a = (e = n(e)) != e, s = null === e, l = $a(e), u = void 0 === e; r < o;) {
@@ -6700,15 +6700,15 @@
                 function nr(t, e, n, i) {
                     return Zi(t, e, n(pi(t, e)), i)
                 }
 
                 function ir(t, e, n, i) {
                     for (var r = t.length, o = i ? r : -1;
                         (i ? o-- : ++o < r) && e(t[o], o, t););
-                    return n ? Yi(t, i ? 0 : o, i ? o + 1 : r) : Yi(t, i ? o + 1 : 0, i ? r : o)
+                    return n ? qi(t, i ? 0 : o, i ? o + 1 : r) : qi(t, i ? o + 1 : 0, i ? r : o)
                 }
 
                 function rr(t, e) {
                     var n = t;
                     return n instanceof Tn && (n = n.value()), ge(e, (function(t, e) {
                         return e.func.apply(e.thisArg, me([t], e.args))
                     }), n)
@@ -6731,28 +6731,28 @@
                 }
 
                 function sr(t) {
                     return Ba(t) ? t : []
                 }
 
                 function lr(t) {
-                    return "function" == typeof t ? t : qs
+                    return "function" == typeof t ? t : Ys
                 }
 
                 function ur(t, e) {
                     return Da(t) ? t : ho(t, e) ? [t] : Oo(us(t))
                 }
                 var hr = Ui;
 
                 function cr(t, e, n) {
                     var i = t.length;
-                    return n = void 0 === n ? i : n, !e && n >= i ? t : Yi(t, e, n)
+                    return n = void 0 === n ? i : n, !e && n >= i ? t : qi(t, e, n)
                 }
                 var fr = Oe || function(t) {
-                    return qt.clearTimeout(t)
+                    return Yt.clearTimeout(t)
                 };
 
                 function pr(t, e) {
                     if (e) return t.slice();
                     var n = t.length,
                         i = Nt ? Nt(n) : new t.constructor(n);
                     return t.copy(i), i
@@ -6814,15 +6814,15 @@
                         void 0 === l && (l = t[s]), r ? Qn(n, s, l) : Vn(n, s, l)
                     }
                     return n
                 }
 
                 function Mr(t, e) {
                     return function(n, i) {
-                        var r = Da(n) ? se : Yn,
+                        var r = Da(n) ? se : qn,
                             o = e ? e() : {};
                         return r(n, t, Xr(i, 2), o)
                     }
                 }
 
                 function wr(t) {
                     return Ui((function(e, n) {
@@ -6856,15 +6856,15 @@
                         }
                         return e
                     }
                 }
 
                 function Ar(t) {
                     return function(e) {
-                        var n = Fe(e = us(e)) ? qe(e) : void 0,
+                        var n = Fe(e = us(e)) ? Ye(e) : void 0,
                             i = n ? n[0] : e.charAt(0),
                             r = n ? cr(n, 1).join("") : e.slice(1);
                         return i[t]() + r
                     }
                 }
 
                 function kr(t) {
@@ -6952,15 +6952,15 @@
                             w = Ne(v, M);
                         if (r && (v = yr(v, r, o, d)), a && (v = _r(v, a, s, d)), _ -= w, d && _ < h) {
                             var x = We(v, M);
                             return Nr(t, e, Pr, y.placeholder, n, v, x, l, u, h - _)
                         }
                         var L = f ? n : this,
                             A = p ? L[t] : t;
-                        return _ = v.length, l ? v = vo(v, l) : m && _ > 1 && v.reverse(), c && u < _ && (v.length = u), this && this !== qt && this instanceof y && (A = g || Or(A)), A.apply(L, v)
+                        return _ = v.length, l ? v = vo(v, l) : m && _ > 1 && v.reverse(), c && u < _ && (v.length = u), this && this !== Yt && this instanceof y && (A = g || Or(A)), A.apply(L, v)
                     }
                 }
 
                 function Er(t, e) {
                     return function(n, i) {
                         return function(t, e, n, i) {
                             return hi(t, (function(t, r, o) {
@@ -6992,16 +6992,16 @@
                         }))
                     }))
                 }
 
                 function Tr(t, e) {
                     var n = (e = void 0 === e ? " " : $i(e)).length;
                     if (n < 2) return n ? Ri(e, t) : e;
-                    var i = Ri(e, tn(t / Ye(e)));
-                    return Fe(e) ? cr(qe(i), 0, t).join("") : i.slice(0, t)
+                    var i = Ri(e, tn(t / qe(e)));
+                    return Fe(e) ? cr(Ye(i), 0, t).join("") : i.slice(0, t)
                 }
 
                 function Dr(t) {
                     return function(e, n, r) {
                         return r && "number" != typeof r && uo(e, n, r) && (n = r = void 0), e = rs(e), void 0 === n ? (n = e, e = 0) : n = rs(n),
                             function(t, e, n, r) {
                                 for (var o = -1, a = ln(tn((e - t) / (n || 1)), 0), s = i(a); a--;) s[r ? a : ++o] = t, t += n;
@@ -7079,31 +7079,31 @@
                             t[0] = e[0], t[1] = r
                         }(g, m), t = g[0], e = g[1], n = g[2], r = g[3], o = g[4], !(h = g[9] = void 0 === g[9] ? c ? 0 : t.length : ln(g[9] - f, 0)) && 24 & e && (e &= -25), e && 1 != e) y = 8 == e || 16 == e ? function(t, e, n) {
                         var r = Or(t);
                         return function o() {
                             for (var a = arguments.length, s = i(a), l = a, u = Jr(o); l--;) s[l] = arguments[l];
                             var h = a < 3 && s[0] !== u && s[a - 1] !== u ? [] : We(s, u);
                             if ((a -= h.length) < n) return Nr(t, e, Pr, o.placeholder, void 0, s, h, void 0, void 0, n - a);
-                            var c = this && this !== qt && this instanceof o ? r : t;
+                            var c = this && this !== Yt && this instanceof o ? r : t;
                             return ae(c, this, s)
                         }
                     }(t, e, h) : 32 != e && 33 != e || o.length ? Pr.apply(void 0, g) : function(t, e, n, r) {
                         var o = 1 & e,
                             a = Or(t);
                         return function e() {
-                            for (var s = -1, l = arguments.length, u = -1, h = r.length, c = i(h + l), f = this && this !== qt && this instanceof e ? a : t; ++u < h;) c[u] = r[u];
+                            for (var s = -1, l = arguments.length, u = -1, h = r.length, c = i(h + l), f = this && this !== Yt && this instanceof e ? a : t; ++u < h;) c[u] = r[u];
                             for (; l--;) c[u++] = arguments[++s];
                             return ae(f, o ? n : this, c)
                         }
                     }(t, e, n, r);
                     else var y = function(t, e, n) {
                         var i = 1 & e,
                             r = Or(t);
                         return function e() {
-                            var o = this && this !== qt && this instanceof e ? r : t;
+                            var o = this && this !== Yt && this instanceof e ? r : t;
                             return o.apply(i ? n : this, arguments)
                         }
                     }(t, e, n);
                     return Lo((m ? Wi : Mo)(y, g), t, e)
                 }
 
                 function Gr(t, e, n, i) {
@@ -7153,19 +7153,19 @@
                     return o.delete(t), o.delete(e), f
                 }
 
                 function Hr(t) {
                     return xo(yo(t, void 0, zo), t + "")
                 }
 
-                function Yr(t) {
+                function qr(t) {
                     return di(t, ws, no)
                 }
 
-                function qr(t) {
+                function Yr(t) {
                     return di(t, xs, io)
                 }
                 var Qr = bn ? function(t) {
                     return bn.get(t)
                 } : $s;
 
                 function Kr(t) {
@@ -7204,15 +7204,15 @@
                     var n = function(t, e) {
                         return null == t ? void 0 : t[e]
                     }(t, e);
                     return Li(n) ? n : void 0
                 }
                 var no = nn ? function(t) {
                         return null == t ? [] : (t = mt(t), ce(nn(t), (function(e) {
-                            return Yt.call(t, e)
+                            return qt.call(t, e)
                         })))
                     } : al,
                     io = nn ? function(t) {
                         for (var e = []; t;) me(e, no(t)), t = Zt(t);
                         return e
                     } : al,
                     ro = mi;
@@ -7300,15 +7300,15 @@
                             o = -1;
                             for (var l = i(e + 1); ++o < e;) l[o] = r[o];
                             return l[e] = n(s), ae(t, this, l)
                         }
                 }
 
                 function _o(t, e) {
-                    return e.length < 2 ? t : pi(t, Yi(e, 0, -1))
+                    return e.length < 2 ? t : pi(t, qi(e, 0, -1))
                 }
 
                 function vo(t, e) {
                     for (var n = t.length, i = un(e.length, n), r = vr(t); i--;) {
                         var o = e[i];
                         t[i] = lo(o, n) ? r[o] : void 0
                     }
@@ -7316,15 +7316,15 @@
                 }
 
                 function bo(t, e) {
                     if (("constructor" !== e || "function" != typeof t[e]) && "__proto__" != e) return t[e]
                 }
                 var Mo = Ao(Wi),
                     wo = $e || function(t, e) {
-                        return qt.setTimeout(t, e)
+                        return Yt.setTimeout(t, e)
                     },
                     xo = Ao(Vi);
 
                 function Lo(t, e, n) {
                     var i = e + "";
                     return xo(t, function(t, e) {
                         var n = e.length;
@@ -7469,19 +7469,19 @@
 
                 function Vo(t) {
                     return null == t ? t : pn.call(t)
                 }
                 var Ho = Ui((function(t) {
                         return tr(si(t, 1, Ba, !0))
                     })),
-                    Yo = Ui((function(t) {
+                    qo = Ui((function(t) {
                         var e = Fo(t);
                         return Ba(e) && (e = void 0), tr(si(t, 1, Ba, !0), Xr(e, 2))
                     })),
-                    qo = Ui((function(t) {
+                    Yo = Ui((function(t) {
                         var e = Fo(t);
                         return e = "function" == typeof e ? e : void 0, tr(si(t, 1, Ba, !0), void 0, e)
                     }));
 
                 function Qo(t) {
                     if (!t || !t.length) return [];
                     var e = 0;
@@ -7584,15 +7584,15 @@
                 }));
                 var ga = Ui((function(t, e) {
                         if (null == t) return [];
                         var n = e.length;
                         return n > 1 && uo(t, e[0], e[1]) ? e = [] : n > 2 && uo(e[0], e[1], e[2]) && (e = [e[0]]), Ti(t, si(e, 1), [])
                     })),
                     ya = Xe || function() {
-                        return qt.Date.now()
+                        return Yt.Date.now()
                     };
 
                 function _a(t, e, n) {
                     return e = n ? void 0 : e, Fr(t, 128, void 0, void 0, void 0, void 0, e = t && null == e ? t.length : e)
                 }
 
                 function va(t, e) {
@@ -7731,15 +7731,15 @@
                 var Ia = zr(gi),
                     ja = zr((function(t, e) {
                         return t >= e
                     })),
                     Ta = Mi(function() {
                         return arguments
                     }()) ? Mi : function(t) {
-                        return Ha(t) && Lt.call(t, "callee") && !Yt.call(t, "callee")
+                        return Ha(t) && Lt.call(t, "callee") && !qt.call(t, "callee")
                     },
                     Da = i.isArray,
                     za = te ? Ie(te) : function(t) {
                         return Ha(t) && mi(t) == L
                     };
 
                 function Na(t) {
@@ -7778,19 +7778,19 @@
                     var e = o(t);
                     return null != t && ("object" == e || "function" == e)
                 }
 
                 function Ha(t) {
                     return null != t && "object" == o(t)
                 }
-                var Ya = ne ? Ie(ne) : function(t) {
+                var qa = ne ? Ie(ne) : function(t) {
                     return Ha(t) && ro(t) == g
                 };
 
-                function qa(t) {
+                function Ya(t) {
                     return "number" == typeof t || Ha(t) && mi(t) == y
                 }
 
                 function Qa(t) {
                     if (!Ha(t) || mi(t) != _) return !1;
                     var e = Zt(t);
                     if (null === e) return !0;
@@ -7817,15 +7817,15 @@
                 var es = zr(Si),
                     ns = zr((function(t, e) {
                         return t <= e
                     }));
 
                 function is(t) {
                     if (!t) return [];
-                    if (Na(t)) return Xa(t) ? qe(t) : vr(t);
+                    if (Na(t)) return Xa(t) ? Ye(t) : vr(t);
                     if (Xt && t[Xt]) return function(t) {
                         for (var e, n = []; !(e = t.next()).done;) n.push(e.value);
                         return n
                     }(t[Xt]());
                     var e = ro(t);
                     return (e == g ? Ge : e == b ? Ve : Es)(t)
                 }
@@ -7902,15 +7902,15 @@
                 }
 
                 function _s(t, e) {
                     return null != t && oo(t, e, _i)
                 }
                 var vs = Er((function(t, e, n) {
                         null != e && "function" != typeof e.toString && (e = Ot.call(e)), t[e] = n
-                    }), Vs(qs)),
+                    }), Vs(Ys)),
                     bs = Er((function(t, e, n) {
                         null != e && "function" != typeof e.toString && (e = Ot.call(e)), Lt.call(t, e) ? t[e].push(n) : t[e] = [n]
                     }), Xr),
                     Ms = Ui(bi);
 
                 function ws(t) {
                     return Na(t) ? Un(t) : ki(t)
@@ -7927,29 +7927,29 @@
                     })),
                     ks = Hr((function(t, e) {
                         var n = {};
                         if (null == t) return n;
                         var i = !1;
                         e = de(e, (function(e) {
                             return e = ur(e, t), i || (i = e.length > 1), e
-                        })), br(t, qr(t), n), i && (n = Xn(n, 7, Wr));
+                        })), br(t, Yr(t), n), i && (n = Xn(n, 7, Wr));
                         for (var r = e.length; r--;) er(n, e[r]);
                         return n
                     }));
                 var Os = Hr((function(t, e) {
                     return null == t ? {} : function(t, e) {
                         return Di(t, e, (function(e, n) {
                             return _s(t, n)
                         }))
                     }(t, e)
                 }));
 
                 function Ss(t, e) {
                     if (null == t) return {};
-                    var n = de(qr(t), (function(t) {
+                    var n = de(Yr(t), (function(t) {
                         return [t]
                     }));
                     return e = Xr(e), Di(t, n, (function(t, n) {
                         return e(t, n[0])
                     }))
                 }
                 var Cs = Ur(ws),
@@ -8011,17 +8011,17 @@
 
                 function Vs(t) {
                     return function() {
                         return t
                     }
                 }
                 var Hs = Cr(),
-                    Ys = Cr(!0);
+                    qs = Cr(!0);
 
-                function qs(t) {
+                function Ys(t) {
                     return t
                 }
 
                 function Qs(t) {
                     return Ai("function" == typeof t ? t : Xn(t, 1))
                 }
                 var Ks = Ui((function(t, e) {
@@ -8106,15 +8106,15 @@
                     if (!arguments.length) return [];
                     var t = arguments[0];
                     return Da(t) ? t : [t]
                 }, Pn.chain = ia, Pn.chunk = function(t, e, n) {
                     e = (n ? uo(t, e, n) : void 0 === e) ? 1 : ln(os(e), 0);
                     var r = null == t ? 0 : t.length;
                     if (!r || e < 1) return [];
-                    for (var o = 0, a = 0, s = i(tn(r / e)); o < r;) s[a++] = Yi(t, o, o += e);
+                    for (var o = 0, a = 0, s = i(tn(r / e)); o < r;) s[a++] = qi(t, o, o += e);
                     return s
                 }, Pn.compact = function(t) {
                     for (var e = -1, n = null == t ? 0 : t.length, i = 0, r = []; ++e < n;) {
                         var o = t[e];
                         o && (r[i++] = o)
                     }
                     return r
@@ -8140,27 +8140,27 @@
                         var e = ws(t);
                         return function(n) {
                             return $n(n, t, e)
                         }
                     }(Xn(t, 1))
                 }, Pn.constant = Vs, Pn.countBy = aa, Pn.create = function(t, e) {
                     var n = En(t);
-                    return null == e ? n : qn(n, e)
+                    return null == e ? n : Yn(n, e)
                 }, Pn.curry = function t(e, n, i) {
                     var r = Fr(e, 8, void 0, void 0, void 0, void 0, void 0, n = i ? void 0 : n);
                     return r.placeholder = t.placeholder, r
                 }, Pn.curryRight = function t(e, n, i) {
                     var r = Fr(e, 16, void 0, void 0, void 0, void 0, void 0, n = i ? void 0 : n);
                     return r.placeholder = t.placeholder, r
                 }, Pn.debounce = wa, Pn.defaults = ms, Pn.defaultsDeep = gs, Pn.defer = xa, Pn.delay = La, Pn.difference = Eo, Pn.differenceBy = Io, Pn.differenceWith = jo, Pn.drop = function(t, e, n) {
                     var i = null == t ? 0 : t.length;
-                    return i ? Yi(t, (e = n || void 0 === e ? 1 : os(e)) < 0 ? 0 : e, i) : []
+                    return i ? qi(t, (e = n || void 0 === e ? 1 : os(e)) < 0 ? 0 : e, i) : []
                 }, Pn.dropRight = function(t, e, n) {
                     var i = null == t ? 0 : t.length;
-                    return i ? Yi(t, 0, (e = i - (e = n || void 0 === e ? 1 : os(e))) < 0 ? 0 : e) : []
+                    return i ? qi(t, 0, (e = i - (e = n || void 0 === e ? 1 : os(e))) < 0 ? 0 : e) : []
                 }, Pn.dropRightWhile = function(t, e) {
                     return t && t.length ? ir(t, Xr(e, 3), !0, !0) : []
                 }, Pn.dropWhile = function(t, e) {
                     return t && t.length ? ir(t, Xr(e, 3), !0) : []
                 }, Pn.fill = function(t, e, n, i) {
                     var r = null == t ? 0 : t.length;
                     return r ? (n && "number" != typeof n && uo(t, e, n) && (n = 0, i = r), function(t, e, n, i) {
@@ -8178,26 +8178,26 @@
                     return n = void 0 === n ? 1 : os(n), si(da(t, e), n)
                 }, Pn.flatten = zo, Pn.flattenDeep = function(t) {
                     return (null == t ? 0 : t.length) ? si(t, 1 / 0) : []
                 }, Pn.flattenDepth = function(t, e) {
                     return (null == t ? 0 : t.length) ? si(t, e = void 0 === e ? 1 : os(e)) : []
                 }, Pn.flip = function(t) {
                     return Fr(t, 512)
-                }, Pn.flow = Hs, Pn.flowRight = Ys, Pn.fromPairs = function(t) {
+                }, Pn.flow = Hs, Pn.flowRight = qs, Pn.fromPairs = function(t) {
                     for (var e = -1, n = null == t ? 0 : t.length, i = {}; ++e < n;) {
                         var r = t[e];
                         i[r[0]] = r[1]
                     }
                     return i
                 }, Pn.functions = function(t) {
                     return null == t ? [] : fi(t, ws(t))
                 }, Pn.functionsIn = function(t) {
                     return null == t ? [] : fi(t, xs(t))
                 }, Pn.groupBy = ca, Pn.initial = function(t) {
-                    return (null == t ? 0 : t.length) ? Yi(t, 0, -1) : []
+                    return (null == t ? 0 : t.length) ? qi(t, 0, -1) : []
                 }, Pn.intersection = Bo, Pn.intersectionBy = Ro, Pn.intersectionWith = Uo, Pn.invert = vs, Pn.invertBy = bs, Pn.invokeMap = fa, Pn.iteratee = Qs, Pn.keyBy = pa, Pn.keys = ws, Pn.keysIn = xs, Pn.map = da, Pn.mapKeys = function(t, e) {
                     var n = {};
                     return e = Xr(e, 3), hi(t, (function(t, i, r) {
                         Qn(n, e(t, i, r), t)
                     })), n
                 }, Pn.mapValues = function(t, e) {
                     var n = {};
@@ -8248,36 +8248,36 @@
                     return null == t ? t : Zi(t, e, n)
                 }, Pn.setWith = function(t, e, n, i) {
                     return i = "function" == typeof i ? i : void 0, null == t ? t : Zi(t, e, n, i)
                 }, Pn.shuffle = function(t) {
                     return (Da(t) ? Zn : Hi)(t)
                 }, Pn.slice = function(t, e, n) {
                     var i = null == t ? 0 : t.length;
-                    return i ? (n && "number" != typeof n && uo(t, e, n) ? (e = 0, n = i) : (e = null == e ? 0 : os(e), n = void 0 === n ? i : os(n)), Yi(t, e, n)) : []
+                    return i ? (n && "number" != typeof n && uo(t, e, n) ? (e = 0, n = i) : (e = null == e ? 0 : os(e), n = void 0 === n ? i : os(n)), qi(t, e, n)) : []
                 }, Pn.sortBy = ga, Pn.sortedUniq = function(t) {
                     return t && t.length ? Ji(t) : []
                 }, Pn.sortedUniqBy = function(t, e) {
                     return t && t.length ? Ji(t, Xr(e, 2)) : []
                 }, Pn.split = function(t, e, n) {
-                    return n && "number" != typeof n && uo(t, e, n) && (e = n = void 0), (n = void 0 === n ? 4294967295 : n >>> 0) ? (t = us(t)) && ("string" == typeof e || null != e && !Ka(e)) && !(e = $i(e)) && Fe(t) ? cr(qe(t), 0, n) : t.split(e, n) : []
+                    return n && "number" != typeof n && uo(t, e, n) && (e = n = void 0), (n = void 0 === n ? 4294967295 : n >>> 0) ? (t = us(t)) && ("string" == typeof e || null != e && !Ka(e)) && !(e = $i(e)) && Fe(t) ? cr(Ye(t), 0, n) : t.split(e, n) : []
                 }, Pn.spread = function(t, e) {
                     if ("function" != typeof t) throw new _t(a);
                     return e = null == e ? 0 : ln(os(e), 0), Ui((function(n) {
                         var i = n[e],
                             r = cr(n, 0, e);
                         return i && me(r, i), ae(t, this, r)
                     }))
                 }, Pn.tail = function(t) {
                     var e = null == t ? 0 : t.length;
-                    return e ? Yi(t, 1, e) : []
+                    return e ? qi(t, 1, e) : []
                 }, Pn.take = function(t, e, n) {
-                    return t && t.length ? Yi(t, 0, (e = n || void 0 === e ? 1 : os(e)) < 0 ? 0 : e) : []
+                    return t && t.length ? qi(t, 0, (e = n || void 0 === e ? 1 : os(e)) < 0 ? 0 : e) : []
                 }, Pn.takeRight = function(t, e, n) {
                     var i = null == t ? 0 : t.length;
-                    return i ? Yi(t, (e = i - (e = n || void 0 === e ? 1 : os(e))) < 0 ? 0 : e, i) : []
+                    return i ? qi(t, (e = i - (e = n || void 0 === e ? 1 : os(e))) < 0 ? 0 : e, i) : []
                 }, Pn.takeRightWhile = function(t, e) {
                     return t && t.length ? ir(t, Xr(e, 3), !1, !0) : []
                 }, Pn.takeWhile = function(t, e) {
                     return t && t.length ? ir(t, Xr(e, 3)) : []
                 }, Pn.tap = function(t, e) {
                     return e(t), t
                 }, Pn.throttle = function(t, e, n) {
@@ -8299,15 +8299,15 @@
                         n = r ? i ? new o : [] : Va(t) && Ga(o) ? En(Zt(t)) : {}
                     }
                     return (r ? le : hi)(t, (function(t, i, r) {
                         return e(n, t, i, r)
                     })), n
                 }, Pn.unary = function(t) {
                     return _a(t, 1)
-                }, Pn.union = Ho, Pn.unionBy = Yo, Pn.unionWith = qo, Pn.uniq = function(t) {
+                }, Pn.union = Ho, Pn.unionBy = qo, Pn.unionWith = Yo, Pn.uniq = function(t) {
                     return t && t.length ? tr(t) : []
                 }, Pn.uniqBy = function(t, e) {
                     return t && t.length ? tr(t, Xr(e, 2)) : []
                 }, Pn.uniqWith = function(t, e) {
                     return e = "function" == typeof e ? e : void 0, t && t.length ? tr(t, void 0, e) : []
                 }, Pn.unset = function(t, e) {
                     return null == t || er(t, e)
@@ -8341,15 +8341,15 @@
                     t = us(t), e = $i(e);
                     var i = t.length,
                         r = n = void 0 === n ? i : Jn(os(n), 0, i);
                     return (n -= e.length) >= 0 && t.slice(n, r) == e
                 }, Pn.eq = Ea, Pn.escape = function(t) {
                     return (t = us(t)) && U.test(t) ? t.replace(B, Re) : t
                 }, Pn.escapeRegExp = function(t) {
-                    return (t = us(t)) && q.test(t) ? t.replace(Y, "\\$&") : t
+                    return (t = us(t)) && Y.test(t) ? t.replace(q, "\\$&") : t
                 }, Pn.every = function(t, e, n) {
                     var i = Da(t) ? he : ri;
                     return n && uo(t, e, n) && (e = void 0), i(t, Xr(e, 3))
                 }, Pn.find = sa, Pn.findIndex = To, Pn.findKey = function(t, e) {
                     return be(t, Xr(e, 3), hi)
                 }, Pn.findLast = la, Pn.findLastIndex = Do, Pn.findLastKey = function(t, e) {
                     return be(t, Xr(e, 3), ci)
@@ -8359,15 +8359,15 @@
                     return null == t ? t : ui(t, Xr(e, 3), xs)
                 }, Pn.forOwn = function(t, e) {
                     return t && hi(t, Xr(e, 3))
                 }, Pn.forOwnRight = function(t, e) {
                     return t && ci(t, Xr(e, 3))
                 }, Pn.get = ys, Pn.gt = Ia, Pn.gte = ja, Pn.has = function(t, e) {
                     return null != t && oo(t, e, yi)
-                }, Pn.hasIn = _s, Pn.head = No, Pn.identity = qs, Pn.includes = function(t, e, n, i) {
+                }, Pn.hasIn = _s, Pn.head = No, Pn.identity = Ys, Pn.includes = function(t, e, n, i) {
                     t = Na(t) ? t : Es(t), n = n && !i ? os(n) : 0;
                     var r = t.length;
                     return n < 0 && (n = ln(r + n, 0)), Xa(t) ? n <= r && t.indexOf(e, n) > -1 : !!r && we(t, e, n) > -1
                 }, Pn.indexOf = function(t, e, n) {
                     var i = null == t ? 0 : t.length;
                     if (!i) return -1;
                     var r = null == n ? 0 : os(n);
@@ -8393,28 +8393,28 @@
                 }, Pn.isEqual = function(t, e) {
                     return wi(t, e)
                 }, Pn.isEqualWith = function(t, e, n) {
                     var i = (n = "function" == typeof n ? n : void 0) ? n(t, e) : void 0;
                     return void 0 === i ? wi(t, e, void 0, n) : !!i
                 }, Pn.isError = Fa, Pn.isFinite = function(t) {
                     return "number" == typeof t && on(t)
-                }, Pn.isFunction = Ga, Pn.isInteger = Za, Pn.isLength = Wa, Pn.isMap = Ya, Pn.isMatch = function(t, e) {
+                }, Pn.isFunction = Ga, Pn.isInteger = Za, Pn.isLength = Wa, Pn.isMap = qa, Pn.isMatch = function(t, e) {
                     return t === e || xi(t, e, to(e))
                 }, Pn.isMatchWith = function(t, e, n) {
                     return n = "function" == typeof n ? n : void 0, xi(t, e, to(e), n)
                 }, Pn.isNaN = function(t) {
-                    return qa(t) && t != +t
+                    return Ya(t) && t != +t
                 }, Pn.isNative = function(t) {
                     if (fo(t)) throw new K("Unsupported core-js use. Try https://npms.io/search?q=ponyfill.");
                     return Li(t)
                 }, Pn.isNil = function(t) {
                     return null == t
                 }, Pn.isNull = function(t) {
                     return null === t
-                }, Pn.isNumber = qa, Pn.isObject = Va, Pn.isObjectLike = Ha, Pn.isPlainObject = Qa, Pn.isRegExp = Ka, Pn.isSafeInteger = function(t) {
+                }, Pn.isNumber = Ya, Pn.isObject = Va, Pn.isObjectLike = Ha, Pn.isPlainObject = Qa, Pn.isRegExp = Ka, Pn.isSafeInteger = function(t) {
                     return Za(t) && t >= -9007199254740991 && t <= 9007199254740991
                 }, Pn.isSet = Ja, Pn.isString = Xa, Pn.isSymbol = $a, Pn.isTypedArray = ts, Pn.isUndefined = function(t) {
                     return void 0 === t
                 }, Pn.isWeakMap = function(t) {
                     return Ha(t) && ro(t) == x
                 }, Pn.isWeakSet = function(t) {
                     return Ha(t) && "[object WeakSet]" == mi(t)
@@ -8426,48 +8426,48 @@
                     var r = i;
                     return void 0 !== n && (r = (r = os(n)) < 0 ? ln(i + r, 0) : un(r, i - 1)), e == e ? function(t, e, n) {
                         for (var i = n + 1; i--;)
                             if (t[i] === e) return i;
                         return i
                     }(t, e, r) : Me(t, Le, r, !0)
                 }, Pn.lowerCase = zs, Pn.lowerFirst = Ns, Pn.lt = es, Pn.lte = ns, Pn.max = function(t) {
-                    return t && t.length ? oi(t, qs, gi) : void 0
+                    return t && t.length ? oi(t, Ys, gi) : void 0
                 }, Pn.maxBy = function(t, e) {
                     return t && t.length ? oi(t, Xr(e, 2), gi) : void 0
                 }, Pn.mean = function(t) {
-                    return Ae(t, qs)
+                    return Ae(t, Ys)
                 }, Pn.meanBy = function(t, e) {
                     return Ae(t, Xr(e, 2))
                 }, Pn.min = function(t) {
-                    return t && t.length ? oi(t, qs, Si) : void 0
+                    return t && t.length ? oi(t, Ys, Si) : void 0
                 }, Pn.minBy = function(t, e) {
                     return t && t.length ? oi(t, Xr(e, 2), Si) : void 0
                 }, Pn.stubArray = al, Pn.stubFalse = sl, Pn.stubObject = function() {
                     return {}
                 }, Pn.stubString = function() {
                     return ""
                 }, Pn.stubTrue = function() {
                     return !0
                 }, Pn.multiply = pl, Pn.nth = function(t, e) {
                     return t && t.length ? ji(t, os(e)) : void 0
                 }, Pn.noConflict = function() {
-                    return qt._ === this && (qt._ = Ct), this
+                    return Yt._ === this && (Yt._ = Ct), this
                 }, Pn.noop = $s, Pn.now = ya, Pn.pad = function(t, e, n) {
                     t = us(t);
-                    var i = (e = os(e)) ? Ye(t) : 0;
+                    var i = (e = os(e)) ? qe(t) : 0;
                     if (!e || i >= e) return t;
                     var r = (e - i) / 2;
                     return Tr(en(r), n) + t + Tr(tn(r), n)
                 }, Pn.padEnd = function(t, e, n) {
                     t = us(t);
-                    var i = (e = os(e)) ? Ye(t) : 0;
+                    var i = (e = os(e)) ? qe(t) : 0;
                     return e && i < e ? t + Tr(e - i, n) : t
                 }, Pn.padStart = function(t, e, n) {
                     t = us(t);
-                    var i = (e = os(e)) ? Ye(t) : 0;
+                    var i = (e = os(e)) ? qe(t) : 0;
                     return e && i < e ? Tr(e - i, n) + t : t
                 }, Pn.parseInt = function(t, e, n) {
                     return n || null == e ? e = 0 : e && (e = +e), cn(us(t).replace(Q, ""), e || 0)
                 }, Pn.random = function(t, e, n) {
                     if (n && "boolean" != typeof n && uo(t, e, n) && (e = n = void 0), void 0 === n && ("boolean" == typeof e ? (n = e, e = void 0) : "boolean" == typeof t && (n = t, t = void 0)), void 0 === t && void 0 === e ? (t = 0, e = 1) : (t = rs(t), void 0 === e ? (e = t, t = 0) : e = rs(e)), t > e) {
                         var i = t;
                         t = e, e = i
@@ -8499,19 +8499,19 @@
                         void 0 === o && (i = r, o = n), t = Ga(o) ? o.call(t) : o
                     }
                     return t
                 }, Pn.round = dl, Pn.runInContext = t, Pn.sample = function(t) {
                     return (Da(t) ? Fn : Fi)(t)
                 }, Pn.size = function(t) {
                     if (null == t) return 0;
-                    if (Na(t)) return Xa(t) ? Ye(t) : t.length;
+                    if (Na(t)) return Xa(t) ? qe(t) : t.length;
                     var e = ro(t);
                     return e == g || e == b ? t.size : ki(t).length
                 }, Pn.snakeCase = Bs, Pn.some = function(t, e, n) {
-                    var i = Da(t) ? _e : qi;
+                    var i = Da(t) ? _e : Yi;
                     return n && uo(t, e, n) && (e = void 0), i(t, Xr(e, 3))
                 }, Pn.sortedIndex = function(t, e) {
                     return Qi(t, e)
                 }, Pn.sortedIndexBy = function(t, e, n) {
                     return Ki(t, e, Xr(n, 2))
                 }, Pn.sortedIndexOf = function(t, e) {
                     var n = null == t ? 0 : t.length;
@@ -8529,15 +8529,15 @@
                         var n = Qi(t, e, !0) - 1;
                         if (Ea(t[n], e)) return n
                     }
                     return -1
                 }, Pn.startCase = Rs, Pn.startsWith = function(t, e, n) {
                     return t = us(t), n = null == n ? 0 : Jn(os(n), 0, t.length), e = $i(e), t.slice(n, n + e.length) == e
                 }, Pn.subtract = ml, Pn.sum = function(t) {
-                    return t && t.length ? Ce(t, qs) : 0
+                    return t && t.length ? Ce(t, Ys) : 0
                 }, Pn.sumBy = function(t, e) {
                     return t && t.length ? Ce(t, Xr(e, 2)) : 0
                 }, Pn.template = function(t, e, n) {
                     var i = Pn.templateSettings;
                     n && uo(t, e, n) && (e = void 0), t = us(t), e = fs({}, e, i, Gr);
                     var r, o, a = fs({}, e.imports, i.imports, Gr),
                         s = ws(a),
@@ -8572,41 +8572,41 @@
                 }, Pn.toNumber = ss, Pn.toSafeInteger = function(t) {
                     return t ? Jn(os(t), -9007199254740991, 9007199254740991) : 0 === t ? t : 0
                 }, Pn.toString = us, Pn.toUpper = function(t) {
                     return us(t).toUpperCase()
                 }, Pn.trim = function(t, e, n) {
                     if ((t = us(t)) && (n || void 0 === e)) return Ee(t);
                     if (!t || !(e = $i(e))) return t;
-                    var i = qe(t),
-                        r = qe(e);
+                    var i = Ye(t),
+                        r = Ye(e);
                     return cr(i, De(i, r), ze(i, r) + 1).join("")
                 }, Pn.trimEnd = function(t, e, n) {
                     if ((t = us(t)) && (n || void 0 === e)) return t.slice(0, Qe(t) + 1);
                     if (!t || !(e = $i(e))) return t;
-                    var i = qe(t);
-                    return cr(i, 0, ze(i, qe(e)) + 1).join("")
+                    var i = Ye(t);
+                    return cr(i, 0, ze(i, Ye(e)) + 1).join("")
                 }, Pn.trimStart = function(t, e, n) {
                     if ((t = us(t)) && (n || void 0 === e)) return t.replace(Q, "");
                     if (!t || !(e = $i(e))) return t;
-                    var i = qe(t);
-                    return cr(i, De(i, qe(e))).join("")
+                    var i = Ye(t);
+                    return cr(i, De(i, Ye(e))).join("")
                 }, Pn.truncate = function(t, e) {
                     var n = 30,
                         i = "...";
                     if (Va(e)) {
                         var r = "separator" in e ? e.separator : r;
                         n = "length" in e ? os(e.length) : n, i = "omission" in e ? $i(e.omission) : i
                     }
                     var o = (t = us(t)).length;
                     if (Fe(t)) {
-                        var a = qe(t);
+                        var a = Ye(t);
                         o = a.length
                     }
                     if (n >= o) return t;
-                    var s = n - Ye(i);
+                    var s = n - qe(i);
                     if (s < 1) return i;
                     var l = a ? cr(a, 0, s).join("") : t.slice(0, s);
                     if (void 0 === r) return l + i;
                     if (a && (s += l.length - s), Ka(r)) {
                         if (t.slice(s).search(r)) {
                             var u, h = l;
                             for (r.global || (r = gt(r.source, us(rt.exec(r)) + "g")), r.lastIndex = 0; u = r.exec(h);) var c = u.index;
@@ -8656,15 +8656,15 @@
                     }
                 })), le(["initial", "tail"], (function(t, e) {
                     var n = "drop" + (e ? "" : "Right");
                     Tn.prototype[t] = function() {
                         return this.__filtered__ ? new Tn(this) : this[n](1)
                     }
                 })), Tn.prototype.compact = function() {
-                    return this.filter(qs)
+                    return this.filter(Ys)
                 }, Tn.prototype.find = function(t) {
                     return this.filter(t).head()
                 }, Tn.prototype.findLast = function(t) {
                     return this.reverse().find(t)
                 }, Tn.prototype.invokeMap = Ui((function(t, e) {
                     return "function" == typeof t ? new Tn(this) : this.map((function(n) {
                         return bi(n, t, e)
@@ -8833,17 +8833,17 @@
                     return this.thru(Vo)
                 }, Pn.prototype.toJSON = Pn.prototype.valueOf = Pn.prototype.value = function() {
                     return rr(this.__wrapped__, this.__actions__)
                 }, Pn.prototype.first = Pn.prototype.head, Xt && (Pn.prototype[Xt] = function() {
                     return this
                 }), Pn
             }();
-            "object" == o(n(14)) && n(14) ? (qt._ = Je, void 0 === (r = function() {
+            "object" == o(n(14)) && n(14) ? (Yt._ = Je, void 0 === (r = function() {
                 return Je
-            }.call(e, n, e, i)) || (i.exports = r)) : Kt ? ((Kt.exports = Je)._ = Je, Qt._ = Je) : qt._ = Je
+            }.call(e, n, e, i)) || (i.exports = r)) : Kt ? ((Kt.exports = Je)._ = Je, Qt._ = Je) : Yt._ = Je
         }).call(this)
     }).call(this, n(10), n(13)(t))
 }, , , function(t, e, n) {
     "use strict";
     n.d(e, "a", (function() {
         return r
     })), n.d(e, "b", (function() {
@@ -13328,27 +13328,27 @@
                             e && (i = i.filter((function(e) {
                                 return Object.getOwnPropertyDescriptor(t, e).enumerable
                             }))), n.push.apply(n, i)
                         }
                         return n
                     }
 
-                    function Y(t) {
+                    function q(t) {
                         for (var e = 1; e < arguments.length; e++) {
                             var n = null != arguments[e] ? arguments[e] : {};
                             e % 2 ? H(Object(n), !0).forEach((function(e) {
-                                q(t, e, n[e])
+                                Y(t, e, n[e])
                             })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(t, Object.getOwnPropertyDescriptors(n)) : H(Object(n)).forEach((function(e) {
                                 Object.defineProperty(t, e, Object.getOwnPropertyDescriptor(n, e))
                             }))
                         }
                         return t
                     }
 
-                    function q(t, e, n) {
+                    function Y(t, e, n) {
                         return e in t ? Object.defineProperty(t, e, {
                             value: n,
                             enumerable: !0,
                             configurable: !0,
                             writable: !0
                         }) : t[e] = n, t
                     }
@@ -13668,15 +13668,15 @@
                             "object" !== Q(e) && (e = {
                                 name: e
                             });
                             var n = this._btnNameMapping(t);
                             if (!e.name) throw new TypeError("Button has no name");
                             if (this.buttons[e.name]) throw new TypeError("Button with this name already exists");
                             var i = this.map.pm.Draw.createNewDrawInstance(e.name, n);
-                            return e = Y(Y({}, this.buttons[n]._button), e), {
+                            return e = q(q({}, this.buttons[n]._button), e), {
                                 drawInstance: i,
                                 control: this.createCustomControl(e)
                             }
                         },
                         createCustomControl: function(t) {
                             var e, n;
                             if (!t.name) throw new TypeError("Button has no name");
@@ -15264,16 +15264,16 @@
                     function Vt(t, e) {
                         return t[0] === e[0] && t[1] === e[1]
                     }
 
                     function Ht(t, e) {
                         return [(t[0] + e[0]) / 2, (t[1] + e[1]) / 2]
                     }
-                    var Yt = r(2676),
-                        qt = r.n(Yt);
+                    var qt = r(2676),
+                        Yt = r.n(qt);
 
                     function Qt(t) {
                         var e = {
                             type: "Feature"
                         };
                         return e.geometry = t, e
                     }
@@ -15367,15 +15367,15 @@
                             })).filter((function(t) {
                                 return !(e.options.layersToCut && L.Util.isArray(e.options.layersToCut) && e.options.layersToCut.length > 0) || e.options.layersToCut.indexOf(t) > -1
                             })).filter((function(t) {
                                 return !e._layerGroup.hasLayer(t)
                             })).filter((function(e) {
                                 try {
                                     var n = !!Ct(t.toGeoJSON(15), e.toGeoJSON(15)).features.length > 0;
-                                    return n || e instanceof L.Polyline && !(e instanceof L.Polygon) ? n : (i = t.toGeoJSON(15), r = e.toGeoJSON(15), o = Kt(i), a = Kt(r), !(0 === (s = qt().intersection(o.coordinates, a.coordinates)).length || !(1 === s.length ? Xt(s[0]) : $t(s))))
+                                    return n || e instanceof L.Polyline && !(e instanceof L.Polygon) ? n : (i = t.toGeoJSON(15), r = e.toGeoJSON(15), o = Kt(i), a = Kt(r), !(0 === (s = Yt().intersection(o.coordinates, a.coordinates)).length || !(1 === s.length ? Xt(s[0]) : $t(s))))
                                 } catch (t) {
                                     return e instanceof L.Polygon && console.error("You can't cut polygons with self-intersections"), !1
                                 }
                                 var i, r, o, a, s
                             })).forEach((function(n) {
                                 var r;
                                 if (n instanceof L.Polygon) {
@@ -15448,15 +15448,15 @@
                                     layer: u,
                                     originalLayer: n
                                 })
                             }))
                         },
                         _cutLayer: function(t, e) {
                             var n, i, r, o, a, s, l = L.geoJSON();
-                            if (e instanceof L.Polygon) i = e.toGeoJSON(15), r = t.toGeoJSON(15), o = Kt(i), a = Kt(r), n = 0 === (s = qt().difference(o.coordinates, a.coordinates)).length ? null : 1 === s.length ? Xt(s[0]) : $t(s);
+                            if (e instanceof L.Polygon) i = e.toGeoJSON(15), r = t.toGeoJSON(15), o = Kt(i), a = Kt(r), n = 0 === (s = Yt().difference(o.coordinates, a.coordinates)).length ? null : 1 === s.length ? Xt(s[0]) : $t(s);
                             else {
                                 var u = te(e);
                                 u.forEach((function(e) {
                                     var n = Rt(e, t.toGeoJSON(15));
                                     (n && n.features.length > 0 ? L.geoJSON(n) : L.geoJSON(e)).getLayers().forEach((function(e) {
                                         (function(t, e) {
                                             var n = Mt(t),
@@ -20114,30 +20114,30 @@
                     U = i.JSON,
                     F = U && U.stringify,
                     G = m("toPrimitive"),
                     Z = C.f,
                     W = f("symbol-registry"),
                     V = f("symbols"),
                     H = f("op-symbols"),
-                    Y = f("wks"),
-                    q = Object.prototype,
+                    q = f("wks"),
+                    Y = Object.prototype,
                     Q = i.QObject,
                     K = n(49),
                     J = !Q || !Q.prototype || !Q.prototype.findChild,
                     X = o && c((function() {
                         return 7 != A(N({}, "a", {
                             get: function() {
                                 return N(this, "a", {
                                     value: 7
                                 }).a
                             }
                         })).a
                     })) ? function(t, e, n) {
-                        var i = z(q, e);
-                        i && delete q[e], N(t, e, n), i && t !== q && N(q, e, i)
+                        var i = z(Y, e);
+                        i && delete Y[e], N(t, e, n), i && t !== Y && N(Y, e, i)
                     } : N,
                     $ = function(t, e) {
                         var n = V[t] = A(R.prototype);
                         return T(n, {
                             type: "Symbol",
                             tag: t,
                             description: e
@@ -20145,72 +20145,72 @@
                     },
                     tt = K && "symbol" == s(R.iterator) ? function(t) {
                         return "symbol" == s(t)
                     } : function(t) {
                         return Object(t) instanceof R
                     },
                     et = function t(e, n, i) {
-                        return e === q && t(H, n, i), b(e), n = x(n, !0), b(i), r(V, n) ? (i.enumerable ? (r(e, I) && e[I][n] && (e[I][n] = !1), i = A(i, {
+                        return e === Y && t(H, n, i), b(e), n = x(n, !0), b(i), r(V, n) ? (i.enumerable ? (r(e, I) && e[I][n] && (e[I][n] = !1), i = A(i, {
                             enumerable: L(0, !1)
                         })) : (r(e, I) || N(e, I, L(1, {})), e[I][n] = !0), X(e, n, i)) : N(e, n, i)
                     },
                     nt = function(t, e) {
                         b(t);
                         for (var n, i = _(e = w(e)), r = 0, o = i.length; o > r;) et(t, n = i[r++], e[n]);
                         return t
                     },
                     it = function(t) {
                         var e = Z.call(this, t = x(t, !0));
-                        return !(this === q && r(V, t) && !r(H, t)) && (!(e || !r(this, t) || !r(V, t) || r(this, I) && this[I][t]) || e)
+                        return !(this === Y && r(V, t) && !r(H, t)) && (!(e || !r(this, t) || !r(V, t) || r(this, I) && this[I][t]) || e)
                     },
                     rt = function(t, e) {
-                        if (t = w(t), e = x(e, !0), t !== q || !r(V, e) || r(H, e)) {
+                        if (t = w(t), e = x(e, !0), t !== Y || !r(V, e) || r(H, e)) {
                             var n = z(t, e);
                             return !n || !r(V, e) || r(t, I) && t[I][e] || (n.enumerable = !0), n
                         }
                     },
                     ot = function(t) {
                         for (var e, n = B(w(t)), i = [], o = 0; n.length > o;) r(V, e = n[o++]) || r(h, e) || i.push(e);
                         return i
                     },
                     at = function(t) {
-                        for (var e, n = t === q, i = B(n ? H : w(t)), o = [], a = 0; i.length > a;) !r(V, e = i[a++]) || n && !r(q, e) || o.push(V[e]);
+                        for (var e, n = t === Y, i = B(n ? H : w(t)), o = [], a = 0; i.length > a;) !r(V, e = i[a++]) || n && !r(Y, e) || o.push(V[e]);
                         return o
                     };
                 K || (u((R = function() {
                     if (this instanceof R) throw TypeError("Symbol is not a constructor");
                     var t = void 0 === arguments[0] ? void 0 : String(arguments[0]),
                         e = d(t),
                         n = function t(n) {
-                            this === q && t.call(H, n), r(this, I) && r(this[I], e) && (this[I][e] = !1), X(this, e, L(1, n))
+                            this === Y && t.call(H, n), r(this, I) && r(this[I], e) && (this[I][e] = !1), X(this, e, L(1, n))
                         };
-                    return o && J && X(q, e, {
+                    return o && J && X(Y, e, {
                         configurable: !0,
                         set: n
                     }), $(e, t)
                 }).prototype, "toString", (function() {
                     return D(this).tag
                 })), C.f = it, S.f = et, O.f = rt, n(34).f = k.f = ot, n(36).f = at, o && (N(R.prototype, "description", {
                     configurable: !0,
                     get: function() {
                         return D(this).description
                     }
-                }), a || u(q, "propertyIsEnumerable", it, {
+                }), a || u(Y, "propertyIsEnumerable", it, {
                     unsafe: !0
                 })), g.f = function(t) {
                     return $(m(t), t)
                 }), l({
                     global: !0,
                     wrap: !0,
                     forced: !K,
                     sham: !K
                 }, {
                     Symbol: R
                 });
-                for (var st = E(Y), lt = 0; st.length > lt;) y(st[lt++]);
+                for (var st = E(q), lt = 0; st.length > lt;) y(st[lt++]);
                 l({
                     target: "Symbol",
                     stat: !0,
                     forced: !K
                 }, {
                     for: function(t) {
                         return r(W, t += "") ? W[t] : W[t] = R(t)
@@ -27726,18 +27726,18 @@
     function W() {
         if (!B && !(B = "undefined" != typeof crypto && crypto.getRandomValues && crypto.getRandomValues.bind(crypto) || "undefined" != typeof msCrypto && "function" == typeof msCrypto.getRandomValues && msCrypto.getRandomValues.bind(msCrypto))) throw new Error("crypto.getRandomValues() not supported. See https://github.com/uuidjs/uuid#getrandomvalues-not-supported");
         return B(Z)
     }
     var V = /^(?:[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}|00000000-0000-0000-0000-000000000000)$/i;
     for (var H = function(t) {
             return "string" == typeof t && V.test(t)
-        }, Y = [], q = 0; q < 256; ++q) Y.push((q + 256).toString(16).substr(1));
+        }, q = [], Y = 0; Y < 256; ++Y) q.push((Y + 256).toString(16).substr(1));
     var Q = function(t) {
         var e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0,
-            n = (Y[t[e + 0]] + Y[t[e + 1]] + Y[t[e + 2]] + Y[t[e + 3]] + "-" + Y[t[e + 4]] + Y[t[e + 5]] + "-" + Y[t[e + 6]] + Y[t[e + 7]] + "-" + Y[t[e + 8]] + Y[t[e + 9]] + "-" + Y[t[e + 10]] + Y[t[e + 11]] + Y[t[e + 12]] + Y[t[e + 13]] + Y[t[e + 14]] + Y[t[e + 15]]).toLowerCase();
+            n = (q[t[e + 0]] + q[t[e + 1]] + q[t[e + 2]] + q[t[e + 3]] + "-" + q[t[e + 4]] + q[t[e + 5]] + "-" + q[t[e + 6]] + q[t[e + 7]] + "-" + q[t[e + 8]] + q[t[e + 9]] + "-" + q[t[e + 10]] + q[t[e + 11]] + q[t[e + 12]] + q[t[e + 13]] + q[t[e + 14]] + q[t[e + 15]]).toLowerCase();
         if (!H(n)) throw TypeError("Stringified UUID is invalid");
         return n
     };
     var K = function(t, e, n) {
             var i = (t = t || {}).random || (t.rng || W)();
             if (i[6] = 15 & i[6] | 64, i[8] = 63 & i[8] | 128, e) {
                 n = n || 0;
@@ -28577,30 +28577,30 @@
                         if (u) throw r
                     }
                 }
                 return s
             }
         }(t, e) || function(t, e) {
             if (!t) return;
-            if ("string" == typeof t) return Yt(t, e);
+            if ("string" == typeof t) return qt(t, e);
             var n = Object.prototype.toString.call(t).slice(8, -1);
             "Object" === n && t.constructor && (n = t.constructor.name);
             if ("Map" === n || "Set" === n) return Array.from(t);
-            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Yt(t, e)
+            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return qt(t, e)
         }(t, e) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function Yt(t, e) {
+    function qt(t, e) {
         (null == e || e > t.length) && (e = t.length);
         for (var n = 0, i = new Array(e); n < e; n++) i[n] = t[n];
         return i
     }
-    var qt = u.a.icon({
+    var Yt = u.a.icon({
             iconUrl: U,
             iconRetinaUrl: F,
             shadowUrl: G,
             iconAnchor: [12, 41],
             iconSize: [25, 41],
             popupAnchor: [1, -34],
             shadowSize: [41, 41]
@@ -28772,22 +28772,22 @@
                                 return e !== t.layer.feature.properties[h]
                             }))
                         }))
                     }
                 },
                 pointToLayer: function(t, e) {
                     return "marker" === j ? y && t.properties[g] ? u.a.marker(e, {
-                        icon: qt
+                        icon: Yt
                     }).bindTooltip(t.properties[g], {
                         direction: L,
                         permanent: A,
                         sticky: k,
                         className: O
                     }) : u.a.marker(e, {
-                        icon: qt
+                        icon: Yt
                     }) : y && t.properties[g] ? u.a.circleMarker(e, {
                         radius: T
                     }).bindTooltip(t.properties[g], {
                         direction: L,
                         permanent: A,
                         sticky: k,
                         className: O
@@ -29706,27 +29706,27 @@
             e && (i = i.filter((function(e) {
                 return Object.getOwnPropertyDescriptor(t, e).enumerable
             }))), n.push.apply(n, i)
         }
         return n
     }
 
-    function Ye(t) {
+    function qe(t) {
         for (var e = 1; e < arguments.length; e++) {
             var n = null != arguments[e] ? arguments[e] : {};
             e % 2 ? He(Object(n), !0).forEach((function(e) {
-                qe(t, e, n[e])
+                Ye(t, e, n[e])
             })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(t, Object.getOwnPropertyDescriptors(n)) : He(Object(n)).forEach((function(e) {
                 Object.defineProperty(t, e, Object.getOwnPropertyDescriptor(n, e))
             }))
         }
         return t
     }
 
-    function qe(t, e, n) {
+    function Ye(t, e, n) {
         var i;
         return i = function(t, e) {
             if ("object" != Ve(t) || !t) return t;
             var n = t[Symbol.toPrimitive];
             if (void 0 !== n) {
                 var i = n.call(t, e || "default");
                 if ("object" != Ve(i)) return i;
@@ -29752,27 +29752,27 @@
             c = t.editable,
             f = t.nClicks,
             p = t.mouseOverCount,
             d = t.loading_state,
             m = t.setProps,
             g = Object(i.useRef)(null);
         return Object(i.useEffect)((function() {
-            g.current && (u ? (Object(J.isBoolean)(u) ? g.current.arrowheads() : g.current.arrowheads(Ye(Ye({}, u), h)), g.current._update()) : g.current.deleteArrowheads())
+            g.current && (u ? (Object(J.isBoolean)(u) ? g.current.arrowheads() : g.current.arrowheads(qe(qe({}, u), h)), g.current._update()) : g.current.deleteArrowheads())
         }), [u]), Object(i.useEffect)((function() {
             g.current && c && g.current.on("pm:edit", (function(t) {
                 m({
                     positions: t.layer._latlngs
                 })
             }))
         }), [c]), r.a.createElement(We, {
             id: e,
             key: n,
             className: o,
             positions: s,
-            pathOptions: Ye(Ye({}, l), {}, {
+            pathOptions: qe(qe({}, l), {}, {
                 pmIgnore: !c
             }),
             ref: g,
             eventHandlers: {
                 click: function() {
                     m({
                         nClicks: f + 1
@@ -30265,28 +30265,28 @@
             return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         })(t)
     }
     var Vn = function(t) {
             return "symbol" == Wn(t) || Zn(t) && "[object Symbol]" == Fn(t)
         },
         Hn = /^[-+]0x[0-9a-f]+$/i,
-        Yn = /^0b[01]+$/i,
-        qn = /^0o[0-7]+$/i,
+        qn = /^0b[01]+$/i,
+        Yn = /^0o[0-7]+$/i,
         Qn = parseInt;
     var Kn = function(t) {
             if ("number" == typeof t) return t;
             if (Vn(t)) return NaN;
             if (wn(t)) {
                 var e = "function" == typeof t.valueOf ? t.valueOf() : t;
                 t = wn(e) ? e + "" : e
             }
             if ("string" != typeof t) return 0 === t ? t : +t;
             t = En(t);
-            var n = Yn.test(t);
-            return n || qn.test(t) ? Qn(t.slice(2), n ? 2 : 8) : Hn.test(t) ? NaN : +t
+            var n = qn.test(t);
+            return n || Yn.test(t) ? Qn(t.slice(2), n ? 2 : 8) : Hn.test(t) ? NaN : +t
         },
         Jn = Math.max,
         Xn = Math.min;
     var $n = function(t, e, n) {
             var i, r, o, a, s, l, u = 0,
                 h = !1,
                 c = !1,
@@ -31197,15 +31197,15 @@
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : t[e] = n, t
     }
 
-    function Yi(t, e) {
+    function qi(t, e) {
         return function(t) {
             if (Array.isArray(t)) return t
         }(t) || function(t, e) {
             var n = null == t ? null : "undefined" != typeof Symbol && t[Symbol.iterator] || t["@@iterator"];
             if (null != n) {
                 var i, r, o, a, s = [],
                     l = !0,
@@ -31225,40 +31225,40 @@
                         if (u) throw r
                     }
                 }
                 return s
             }
         }(t, e) || function(t, e) {
             if (!t) return;
-            if ("string" == typeof t) return qi(t, e);
+            if ("string" == typeof t) return Yi(t, e);
             var n = Object.prototype.toString.call(t).slice(8, -1);
             "Object" === n && t.constructor && (n = t.constructor.name);
             if ("Map" === n || "Set" === n) return Array.from(t);
-            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return qi(t, e)
+            if ("Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Yi(t, e)
         }(t, e) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function qi(t, e) {
+    function Yi(t, e) {
         (null == e || e > t.length) && (e = t.length);
         for (var n = 0, i = new Array(e); n < e; n++) i[n] = t[n];
         return i
     }
     var Qi = function(t) {
         var e = t.positions,
             n = t.pathOptions,
             o = t.paused,
             a = t.reverse,
             s = t.hardwareAccelerated,
             l = t.pulseColor,
             u = t.delay,
             h = t.dashArray,
             c = Object(X.a)(),
-            f = Yi(Object(i.useState)(null), 2),
+            f = qi(Object(i.useState)(null), 2),
             p = f[0],
             d = f[1];
         return Object(i.useEffect)((function() {
             c && (p && p.remove(), d(Object(Gi.antPath)(e, Object(J.omitBy)(Vi(Vi({}, n), {}, {
                 pmIgnore: !0,
                 paused: o,
                 reverse: a,
@@ -32337,57 +32337,57 @@
             l.current && Wr(u.current, r) && Wr(l.current.options, s) || (l.current = new Nr(s), l.current.load(r)), o && f(l.current.getClusters(o, p)), u.current = r
         }, n = [r, o, p, s], i.useEffect(e, Vr(n)), {
             clusters: c,
             supercluster: l.current
         }
     };
 
-    function Yr(t) {
-        return (Yr = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+    function qr(t) {
+        return (qr = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
             return typeof t
         } : function(t) {
             return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
         })(t)
     }
 
-    function qr(t, e) {
+    function Yr(t, e) {
         var n = Object.keys(t);
         if (Object.getOwnPropertySymbols) {
             var i = Object.getOwnPropertySymbols(t);
             e && (i = i.filter((function(e) {
                 return Object.getOwnPropertyDescriptor(t, e).enumerable
             }))), n.push.apply(n, i)
         }
         return n
     }
 
     function Qr(t) {
         for (var e = 1; e < arguments.length; e++) {
             var n = null != arguments[e] ? arguments[e] : {};
-            e % 2 ? qr(Object(n), !0).forEach((function(e) {
+            e % 2 ? Yr(Object(n), !0).forEach((function(e) {
                 Kr(t, e, n[e])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(t, Object.getOwnPropertyDescriptors(n)) : qr(Object(n)).forEach((function(e) {
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(t, Object.getOwnPropertyDescriptors(n)) : Yr(Object(n)).forEach((function(e) {
                 Object.defineProperty(t, e, Object.getOwnPropertyDescriptor(n, e))
             }))
         }
         return t
     }
 
     function Kr(t, e, n) {
         var i;
         return i = function(t, e) {
-            if ("object" != Yr(t) || !t) return t;
+            if ("object" != qr(t) || !t) return t;
             var n = t[Symbol.toPrimitive];
             if (void 0 !== n) {
                 var i = n.call(t, e || "default");
-                if ("object" != Yr(i)) return i;
+                if ("object" != qr(i)) return i;
                 throw new TypeError("@@toPrimitive must return a primitive value.")
             }
             return ("string" === e ? String : Number)(t)
-        }(e, "string"), (e = "symbol" == Yr(i) ? i : String(i)) in t ? Object.defineProperty(t, e, {
+        }(e, "string"), (e = "symbol" == qr(i) ? i : String(i)) in t ? Object.defineProperty(t, e, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : t[e] = n, t
     }
 
@@ -33332,21 +33332,21 @@
 
     function Ho(t, e, n, i) {
         var r = Zo(e),
             o = Wo(n, i),
             a = (t + "?" + r).length;
         if (a <= 2e3 && Uo.cors ? o.open("GET", t + "?" + r) : a > 2e3 && Uo.cors && (o.open("POST", t), o.setRequestHeader("Content-Type", "application/x-www-form-urlencoded; charset=UTF-8")), null != i && void 0 !== i.options && (o.timeout = i.options.timeout, i.options.withCredentials && (o.withCredentials = !0)), a <= 2e3 && Uo.cors) o.send(null);
         else {
-            if (!(a > 2e3 && Uo.cors)) return a <= 2e3 && !Uo.cors ? Yo(t, e, n, i) : void Qo("a request to " + t + " was longer then 2000 characters and this browser cannot make a cross-domain post request. Please use a proxy https://developers.arcgis.com/esri-leaflet/api-reference/request/");
+            if (!(a > 2e3 && Uo.cors)) return a <= 2e3 && !Uo.cors ? qo(t, e, n, i) : void Qo("a request to " + t + " was longer then 2000 characters and this browser cannot make a cross-domain post request. Please use a proxy https://developers.arcgis.com/esri-leaflet/api-reference/request/");
             o.send(r)
         }
         return o
     }
 
-    function Yo(t, e, n, i) {
+    function qo(t, e, n, i) {
         window._EsriLeafletCallbacks = window._EsriLeafletCallbacks || {};
         var r = "c" + Go;
         e.callback = "window._EsriLeafletCallbacks." + r, window._EsriLeafletCallbacks[r] = function(t) {
             if (!0 !== window._EsriLeafletCallbacks[r]) {
                 var e, o = Object.prototype.toString.call(t);
                 "[object Object]" !== o && "[object Array]" !== o && (e = {
                     error: {
@@ -33373,23 +33373,23 @@
                 window._EsriLeafletCallbacks._callback[r]({
                     code: 0,
                     message: "Request aborted."
                 })
             }
         }
     }
-    var qo = Uo.cors ? Vo : Yo;
+    var Yo = Uo.cors ? Vo : qo;
 
     function Qo() {
         console && console.warn && console.warn.apply(console, arguments)
     }
-    qo.CORS = Vo, qo.JSONP = Yo;
+    Yo.CORS = Vo, Yo.JSONP = qo;
     var Ko = {
             request: Ho,
-            get: qo,
+            get: Yo,
             post: function(t, e, n, i) {
                 var r = Wo(n, i);
                 return r.open("POST", t), null != i && void 0 !== i.options && (r.timeout = i.options.timeout), r.setRequestHeader("Content-Type", "application/x-www-form-urlencoded; charset=UTF-8"), r.send(Zo(e)), r
             }
         },
         Jo = function(t, e, n, i) {
             var r = (i[0] - n[0]) * (t[1] - n[1]) - (i[1] - n[1]) * (t[0] - n[0]),
@@ -34517,15 +34517,15 @@
             onAdd: function(t) {
                 this._topLeft = t.getPixelBounds().min, l.ImageOverlay.prototype.onAdd.call(this, t)
             },
             _reset: function() {
                 this._map.options.crs === l.CRS.EPSG3857 ? l.ImageOverlay.prototype._reset.call(this) : l.DomUtil.setPosition(this._image, this._topLeft.subtract(this._map.getPixelOrigin()))
             }
         }),
-        Ya = l.Layer.extend({
+        qa = l.Layer.extend({
             options: {
                 opacity: 1,
                 position: "front",
                 f: "image",
                 useCors: Bo,
                 attribution: null,
                 interactive: !1,
@@ -34648,15 +34648,15 @@
                     n = this._map.unproject(t.getBottomLeft()),
                     i = this._map.unproject(t.getTopRight()),
                     r = this._map.latLngToLayerPoint(i).y,
                     o = this._map.latLngToLayerPoint(n).y;
                 return (r > 0 || o < e.y) && (e.y = o - r), e.x + "," + e.y
             }
         });
-    Ya.extend({
+    qa.extend({
         options: {
             updateInterval: 150,
             format: "jpgpng",
             transparent: !0,
             f: "image"
         },
         query: function() {
@@ -34729,15 +34729,15 @@
             else {
                 t.f = "image";
                 var n = this.options.url + "exportImage" + l.Util.getParamString(t);
                 this.options.proxy && (n = this.options.proxy + "?" + n), this._renderImage(n, e)
             }
         }
     });
-    Ya.extend({
+    qa.extend({
         options: {
             updateInterval: 150,
             layers: !1,
             layerDefs: !1,
             timeOptions: !1,
             format: "png32",
             transparent: !0,
@@ -34813,15 +34813,15 @@
             else {
                 t.f = "image";
                 var n = this.options.url + "export" + l.Util.getParamString(t);
                 this.options.proxy && (n = this.options.proxy + "?" + n), this._renderImage(n, e)
             }
         }
     });
-    var qa = l.Layer.extend({
+    var Ya = l.Layer.extend({
         options: {
             cellSize: 512,
             updateWhenIdle: l.Browser.mobile,
             updateInterval: 150,
             noWrap: !1,
             keepBuffer: 1.5
         },
@@ -35075,45 +35075,45 @@
         return this.values = this.values.concat([].concat(t || [])), e ? this.sort() : this.dirty = !0, this
     }, Qa.prototype.sort = function() {
         return this.values.sort((function(t, e) {
             return +e.value - +t.value
         })).reverse(), this.dirty = !1, this
     };
     var Ka = Qa,
-        Ja = qa.extend({
+        Ja = Ya.extend({
             options: {
                 attribution: null,
                 where: "1=1",
                 fields: ["*"],
                 from: !1,
                 to: !1,
                 timeField: !1,
                 timeFilterMode: "server",
                 simplifyFactor: 0,
                 precision: 6,
                 fetchAllFeatures: !1
             },
             initialize: function(t) {
-                if (qa.prototype.initialize.call(this, t), t = ma(t), t = l.Util.setOptions(this, t), this.service = Ua(t), this.service.addEventParent(this), "*" !== this.options.fields[0]) {
+                if (Ya.prototype.initialize.call(this, t), t = ma(t), t = l.Util.setOptions(this, t), this.service = Ua(t), this.service.addEventParent(this), "*" !== this.options.fields[0]) {
                     for (var e = !1, n = 0; n < this.options.fields.length; n++) this.options.fields[n].match(/^(OBJECTID|FID|OID|ID)$/i) && (e = !0);
                     !1 === e && Qo("no known esriFieldTypeOID field detected in fields Array.  Please add an attribute field containing unique IDs to ensure the layer can be drawn correctly.")
                 }
                 this.options.timeField.start && this.options.timeField.end ? (this._startTimeIndex = new Ka, this._endTimeIndex = new Ka) : this.options.timeField && (this._timeIndex = new Ka), this._cache = {}, this._currentSnapshot = [], this._activeRequests = 0
             },
             onAdd: function(t) {
                 return va(t), this.service.metadata((function(e, n) {
                     if (!e) {
                         var i = n.supportedQueryFormats,
                             r = !1;
                         (!1 === this.service.options.isModern || this.options.fetchAllFeatures) && (r = !0), !r && i && -1 !== i.indexOf("geoJSON") && (this.service.options.isModern = !0), n.objectIdField && (this.service.options.idAttribute = n.objectIdField), !this.options.attribution && t.attributionControl && n.copyrightText && (this.options.attribution = n.copyrightText, t.attributionControl.addAttribution(this.getAttribution()))
                     }
-                }), this), t.on("zoomend", this._handleZoomChange, this), qa.prototype.onAdd.call(this, t)
+                }), this), t.on("zoomend", this._handleZoomChange, this), Ya.prototype.onAdd.call(this, t)
             },
             onRemove: function(t) {
-                return ba(t), t.off("zoomend", this._handleZoomChange, this), qa.prototype.onRemove.call(this, t)
+                return ba(t), t.off("zoomend", this._handleZoomChange, this), Ya.prototype.onRemove.call(this, t)
             },
             getAttribution: function() {
                 return this.options.attribution
             },
             createCell: function(t, e) {
                 this._visibleZoom() && this._requestFeatures(t, e)
             },
@@ -35503,27 +35503,32 @@
                 });
                 return f.current = t, t.addTo(c),
                     function() {
                         c.removeLayer(t), f.current = null
                     }
             }
         }), [n, o, a]), Object(i.useEffect)((function() {
-            l && (f.current && f.current.identify().on(c).at([l.position.lat, l.position.lng]).run((function(t, n, i) {
-                u && console.log("identifyResult of : ".concat(e, "\n"), {
-                    featureCollection: n,
-                    timestamp: Date.now()
-                }), h({
-                    identifyResult: {
-                        featureCollection: n,
-                        timestamp: Date.now()
-                    }
+            if (l) {
+                if (f.current) try {
+                    f.current.identify().on(c).at([l.position.lat, l.position.lng]).run((function(t, n, i) {
+                        u && console.log("identifyResult of : ".concat(e, "\n"), {
+                            featureCollection: n,
+                            timestamp: Date.now()
+                        }), h({
+                            identifyResult: {
+                                featureCollection: n,
+                                timestamp: Date.now()
+                            }
+                        })
+                    }))
+                } catch (t) {}
+                h({
+                    identifyConfig: null
                 })
-            })), h({
-                identifyConfig: null
-            }))
+            }
         }), [l]), r.a.createElement(r.a.Fragment, null)
     };
     Xa.propTypes = {
         id: a.a.string,
         key: a.a.string,
         url: a.a.string,
         opacity: a.a.number,
@@ -35633,53 +35638,196 @@
         }),
         setProps: a.a.func
     }, os.defaultProps = {};
     var as = r.a.memo(os),
         ss = function(t) {
             var e = t.id,
                 n = t.groupId,
-                o = (t.setProps, Object(X.a)()),
-                a = Object(i.useContext)(ns);
+                o = t.syncStrategy,
+                a = (t.setProps, Object(X.a)()),
+                s = Object(i.useContext)(ns);
             return Object(i.useEffect)((function() {
-                return o.on("movestart zoomstart", (function(t) {
-                        a.triggerId.current || (a.triggerId.current = e)
-                    })), o.on("move zoom", (function(t) {
-                        a.triggerId.current && a.triggerId.current === e && a.setViewState({
-                            zoom: o.getZoom(),
-                            center: o.getCenter(),
+                return a.on("movestart zoomstart", (function(t) {
+                        s.triggerId.current || (s.triggerId.current = e)
+                    })), a.on("move zoom", (function(t) {
+                        s.triggerId.current && s.triggerId.current === e && s.setViewState({
+                            zoom: a.getZoom(),
+                            center: a.getCenter(),
                             groupId: n,
                             triggerId: e,
                             eventType: t.type
                         })
-                    })), o.on("moveend zoomend", (function(t) {
-                        a.triggerId.current === e && (a.triggerId.current = null)
+                    })), a.on("moveend zoomend", (function(t) {
+                        s.triggerId.current === e && (s.triggerId.current = null)
                     })),
                     function() {
-                        o.off("movestart zoomstart"), o.off("move zoom"), o.off("moveend zoomend")
+                        a.off("movestart zoomstart"), a.off("move zoom"), a.off("moveend zoomend")
                     }
-            }), [o]), Object(i.useEffect)((function() {
-                a.viewState && a.triggerId.current && (a.viewState.groupId && a.viewState.groupId === n ? a.triggerId.current !== e && o.setView(a.viewState.center, a.viewState.zoom, {
-                    animate: "zoom" === a.viewState.eventType
-                }) : a.viewState.groupId || a.triggerId.current !== e && o.setView(a.viewState.center, a.viewState.zoom, {
-                    animate: "zoom" === a.viewState.eventType
+            }), [a]), Object(i.useEffect)((function() {
+                s.viewState && s.triggerId.current && (s.viewState.groupId && s.viewState.groupId === n ? s.triggerId.current !== e && a.setView(s.viewState.center, "all" === o ? s.viewState.zoom : a.getZoom(), {
+                    animate: "zoom" === s.viewState.eventType
+                }) : s.viewState.groupId || s.triggerId.current !== e && a.setView(s.viewState.center, "all" === o ? s.viewState.zoom : a.getZoom(), {
+                    animate: "zoom" === s.viewState.eventType
                 }))
-            }), [a.viewState]), r.a.createElement(r.a.Fragment, null)
+            }), [s.viewState]), r.a.createElement(r.a.Fragment, null)
         };
     ss.propTypes = {
         id: a.a.string.isRequired,
         key: a.a.string,
         groupId: a.a.string,
+        syncStrategy: a.a.oneOf(["all", "center"]),
         loading_state: a.a.shape({
             is_loading: a.a.bool,
             prop_name: a.a.string,
             component_name: a.a.string
         }),
         setProps: a.a.func
-    }, ss.defaultProps = {};
+    }, ss.defaultProps = {
+        syncStrategy: "all"
+    };
     var ls = r.a.memo(ss);
+
+    function us(t) {
+        return (us = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
+            return typeof t
+        } : function(t) {
+            return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
+        })(t)
+    }
+    var hs = ["bounds", "url"];
+
+    function cs(t, e) {
+        var n = Object.keys(t);
+        if (Object.getOwnPropertySymbols) {
+            var i = Object.getOwnPropertySymbols(t);
+            e && (i = i.filter((function(e) {
+                return Object.getOwnPropertyDescriptor(t, e).enumerable
+            }))), n.push.apply(n, i)
+        }
+        return n
+    }
+
+    function fs(t) {
+        for (var e = 1; e < arguments.length; e++) {
+            var n = null != arguments[e] ? arguments[e] : {};
+            e % 2 ? cs(Object(n), !0).forEach((function(e) {
+                ps(t, e, n[e])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(t, Object.getOwnPropertyDescriptors(n)) : cs(Object(n)).forEach((function(e) {
+                Object.defineProperty(t, e, Object.getOwnPropertyDescriptor(n, e))
+            }))
+        }
+        return t
+    }
+
+    function ps(t, e, n) {
+        var i;
+        return i = function(t, e) {
+            if ("object" != us(t) || !t) return t;
+            var n = t[Symbol.toPrimitive];
+            if (void 0 !== n) {
+                var i = n.call(t, e || "default");
+                if ("object" != us(i)) return i;
+                throw new TypeError("@@toPrimitive must return a primitive value.")
+            }
+            return ("string" === e ? String : Number)(t)
+        }(e, "string"), (e = "symbol" == us(i) ? i : String(i)) in t ? Object.defineProperty(t, e, {
+            value: n,
+            enumerable: !0,
+            configurable: !0,
+            writable: !0
+        }) : t[e] = n, t
+    }
+
+    function ds(t, e) {
+        if (null == t) return {};
+        var n, i, r = function(t, e) {
+            if (null == t) return {};
+            var n, i, r = {},
+                o = Object.keys(t);
+            for (i = 0; i < o.length; i++) n = o[i], e.indexOf(n) >= 0 || (r[n] = t[n]);
+            return r
+        }(t, e);
+        if (Object.getOwnPropertySymbols) {
+            var o = Object.getOwnPropertySymbols(t);
+            for (i = 0; i < o.length; i++) n = o[i], e.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(t, n) && (r[n] = t[n])
+        }
+        return r
+    }
+    var ms = j((function(t, e) {
+            var n = t.bounds,
+                i = t.url,
+                r = ds(t, hs),
+                o = new l.ImageOverlay(i, n, r);
+            return {
+                instance: o,
+                context: fs(fs({}, e), {}, {
+                    overlayContainer: o
+                })
+            }
+        }), (function(t, e, n) {
+            ! function(t, e, n) {
+                e.bounds instanceof l.LatLngBounds && e.bounds !== n.bounds && t.setBounds(e.bounds), null != e.opacity && e.opacity !== n.opacity && t.setOpacity(e.opacity), null != e.zIndex && e.zIndex !== n.zIndex && t.setZIndex(e.zIndex)
+            }(t, e, n), e.url !== n.url && t.setUrl(e.url)
+        })),
+        gs = function(t) {
+            var e = t.id,
+                n = t.className,
+                o = t.url,
+                a = t.bounds,
+                s = t.opacity,
+                l = t.zIndex,
+                h = t.minZoom,
+                c = t.maxZoom,
+                f = t.loading_state,
+                p = Object(X.a)(),
+                d = Object(i.useRef)(null);
+            return Object(i.useEffect)((function() {
+                if (p && (h || c)) {
+                    var t = function() {
+                        p.getZoom() >= (h || 0) && p.getZoom() <= (c || 22) ? 0 === s ? d.current.setOpacity(0) : d.current.setOpacity(s || 1) : d.current.setOpacity(0)
+                    };
+                    return p.on("zoomend", t),
+                        function() {
+                            0 === s ? d.current.setOpacity(0) : d.current.setOpacity(s || 1), p.off("zoomend", t)
+                        }
+                }
+            }), [s, h, c]), r.a.createElement(ms, {
+                id: e,
+                className: n,
+                ref: d,
+                url: o,
+                bounds: u.a.latLngBounds(u.a.latLng(a.miny, a.minx), u.a.latLng(a.maxy, a.maxx)),
+                opacity: s,
+                zIndex: l,
+                "data-dash-is-loading": f && f.is_loading || void 0
+            })
+        };
+    gs.propTypes = {
+        id: a.a.string,
+        key: a.a.string,
+        className: a.a.string,
+        url: a.a.string.isRequired,
+        bounds: a.a.exact({
+            minx: a.a.number.isRequired,
+            miny: a.a.number.isRequired,
+            maxx: a.a.number.isRequired,
+            maxy: a.a.number.isRequired
+        }).isRequired,
+        opacity: a.a.number,
+        zIndex: a.a.number,
+        minZoom: a.a.number,
+        maxZoom: a.a.number,
+        loading_state: a.a.shape({
+            is_loading: a.a.bool,
+            prop_name: a.a.string,
+            component_name: a.a.string
+        }),
+        setProps: a.a.func
+    }, gs.defaultProps = {};
+    var ys = r.a.memo(gs);
     n.d(e, "LeafletMap", (function() {
         return St
     })), n.d(e, "LeafletTileLayer", (function() {
         return jt
     })), n.d(e, "LeafletGeoJSON", (function() {
         return te
     })), n.d(e, "LeafletHeatMap", (function() {
@@ -35732,14 +35880,16 @@
         return $a
     })), n.d(e, "Fragment", (function() {
         return es
     })), n.d(e, "LeafletMapProvider", (function() {
         return as
     })), n.d(e, "LeafletMapSync", (function() {
         return ls
+    })), n.d(e, "LeafletImageOverlay", (function() {
+        return ys
     }))
 }, function(t, e, n) {
     "use strict";
     n.r(e);
     var i = 484813681109536e-20,
         r = Math.PI / 2,
         o = .017453292519943295,
@@ -36519,32 +36669,32 @@
         ellipse: "bessel",
         datumName: "Gunung Segara Jakarta"
     }, H.rnb72 = {
         towgs84: "106.869,-52.2978,103.724,-0.33657,0.456955,-1.84218,1",
         ellipse: "intl",
         datumName: "Reseau National Belge 1972"
     };
-    var Y = function(t, e, n, r, o, a, s) {
+    var q = function(t, e, n, r, o, a, s) {
             var l = {};
             return l.datum_type = void 0 === t || "none" === t ? 5 : 4, e && (l.datum_params = e.map(parseFloat), 0 === l.datum_params[0] && 0 === l.datum_params[1] && 0 === l.datum_params[2] || (l.datum_type = 1), l.datum_params.length > 3 && (0 === l.datum_params[3] && 0 === l.datum_params[4] && 0 === l.datum_params[5] && 0 === l.datum_params[6] || (l.datum_type = 2, l.datum_params[3] *= i, l.datum_params[4] *= i, l.datum_params[5] *= i, l.datum_params[6] = l.datum_params[6] / 1e6 + 1))), s && (l.datum_type = 3, l.grids = s), l.a = n, l.b = r, l.es = o, l.ep2 = a, l
         },
-        q = {};
+        Y = {};
 
     function Q(t) {
         if (0 === t.length) return null;
         var e = "@" === t[0];
         return e && (t = t.slice(1)), "null" === t ? {
             name: "null",
             mandatory: !e,
             grid: null,
             isNull: !0
         } : {
             name: t,
             mandatory: !e,
-            grid: q[t] || null,
+            grid: Y[t] || null,
             isNull: !1
         }
     }
 
     function K(t) {
         return t / 3600 * Math.PI / 180
     }
@@ -36624,15 +36774,15 @@
                         es: h,
                         e: c,
                         ep2: (l - u) / u
                     }),
                     m = function(t) {
                         return void 0 === t ? null : t.split(",").map(Q)
                     }(n.nadgrids),
-                    g = n.datum || Y(n.datumCode, n.datum_params, f.a, f.b, d.es, d.ep2, m);
+                    g = n.datum || q(n.datumCode, n.datum_params, f.a, f.b, d.es, d.ep2, m);
                 I(this, n), I(this, i), this.a = f.a, this.b = f.b, this.rf = f.rf, this.sphere = f.sphere, this.es = d.es, this.e = d.e, this.ep2 = d.ep2, this.datum = g, this.init(), e(null, this)
             } else e(t)
         } else e(t)
     }
     nt.projections = Z, nt.projections.start();
     var it = nt;
 
@@ -37365,15 +37515,15 @@
             },
             names: ["Universal Transverse Mercator System", "utm"],
             dependsOn: "etmerc"
         },
         Ht = function(t, e) {
             return Math.pow((1 - t) / (1 + t), e)
         };
-    var Yt = {
+    var qt = {
         init: function() {
             var t = Math.sin(this.lat0),
                 e = Math.cos(this.lat0);
             e *= e, this.rc = Math.sqrt(1 - this.es) / (1 - this.es * t * t), this.C = Math.sqrt(1 + this.es * e * e / (1 - this.es)), this.phic0 = Math.asin(t / this.C), this.ratexp = .5 * this.C * this.e, this.K = Math.tan(.5 * this.phic0 + s) / (Math.pow(Math.tan(.5 * this.lat0 + s), this.C) * Ht(this.e * t, this.ratexp))
         },
         forward: function(t) {
             var e = t.x,
@@ -37382,29 +37532,29 @@
         },
         inverse: function(t) {
             for (var e = t.x / this.C, n = t.y, i = Math.pow(Math.tan(.5 * n + s) / this.K, 1 / this.C), o = 20; o > 0 && (n = 2 * Math.atan(i * Ht(this.e * Math.sin(t.y), -.5 * this.e)) - r, !(Math.abs(n - t.y) < 1e-14)); --o) t.y = n;
             return o ? (t.x = e, t.y = n, t) : null
         },
         names: ["gauss"]
     };
-    var qt = {
+    var Yt = {
         init: function() {
-            Yt.init.apply(this), this.rc && (this.sinc0 = Math.sin(this.phic0), this.cosc0 = Math.cos(this.phic0), this.R2 = 2 * this.rc, this.title || (this.title = "Oblique Stereographic Alternative"))
+            qt.init.apply(this), this.rc && (this.sinc0 = Math.sin(this.phic0), this.cosc0 = Math.cos(this.phic0), this.R2 = 2 * this.rc, this.title || (this.title = "Oblique Stereographic Alternative"))
         },
         forward: function(t) {
             var e, n, i, r;
-            return t.x = D(t.x - this.long0), Yt.forward.apply(this, [t]), e = Math.sin(t.y), n = Math.cos(t.y), i = Math.cos(t.x), r = this.k0 * this.R2 / (1 + this.sinc0 * e + this.cosc0 * n * i), t.x = r * n * Math.sin(t.x), t.y = r * (this.cosc0 * e - this.sinc0 * n * i), t.x = this.a * t.x + this.x0, t.y = this.a * t.y + this.y0, t
+            return t.x = D(t.x - this.long0), qt.forward.apply(this, [t]), e = Math.sin(t.y), n = Math.cos(t.y), i = Math.cos(t.x), r = this.k0 * this.R2 / (1 + this.sinc0 * e + this.cosc0 * n * i), t.x = r * n * Math.sin(t.x), t.y = r * (this.cosc0 * e - this.sinc0 * n * i), t.x = this.a * t.x + this.x0, t.y = this.a * t.y + this.y0, t
         },
         inverse: function(t) {
             var e, n, i, r, o;
             if (t.x = (t.x - this.x0) / this.a, t.y = (t.y - this.y0) / this.a, t.x /= this.k0, t.y /= this.k0, o = Ut(t.x, t.y)) {
                 var a = 2 * Math.atan2(o, this.R2);
                 e = Math.sin(a), n = Math.cos(a), r = Math.asin(n * this.sinc0 + t.y * e * this.cosc0 / o), i = Math.atan2(t.x * e, o * this.cosc0 * n - t.y * this.sinc0 * e)
             } else r = this.phic0, i = 0;
-            return t.x = i, t.y = r, Yt.inverse.apply(this, [t]), t.x = D(t.x + this.long0), t
+            return t.x = i, t.y = r, qt.inverse.apply(this, [t]), t.x = D(t.x + this.long0), t
         },
         names: ["Stereographic_North_Pole", "Oblique_Stereographic", "sterea", "Oblique Stereographic Alternative", "Double_Stereographic"]
     };
     var Qt = {
         init: function() {
             this.x0 = this.x0 || 0, this.y0 = this.y0 || 0, this.lat0 = this.lat0 || 0, this.long0 = this.long0 || 0, this.coslat0 = Math.cos(this.lat0), this.sinlat0 = Math.sin(this.lat0), this.sphere ? 1 === this.k0 && !isNaN(this.lat_ts) && Math.abs(this.coslat0) <= 1e-10 && (this.k0 = .5 * (1 + T(this.lat0) * Math.sin(this.lat_ts))) : (Math.abs(this.coslat0) <= 1e-10 && (this.lat0 > 0 ? this.con = 1 : this.con = -1), this.cons = Math.sqrt(Math.pow(1 + this.e, 1 + this.e) * Math.pow(1 - this.e, 1 - this.e)), 1 === this.k0 && !isNaN(this.lat_ts) && Math.abs(this.coslat0) <= 1e-10 && Math.abs(Math.cos(this.lat_ts)) > 1e-10 && (this.k0 = .5 * this.cons * j(this.e, Math.sin(this.lat_ts), Math.cos(this.lat_ts)) / z(this.e, this.con * this.lat_ts, this.con * Math.sin(this.lat_ts))), this.ms1 = j(this.e, this.sinlat0, this.coslat0), this.X0 = 2 * Math.atan(this.ssfn_(this.lat0, this.sinlat0, this.e)) - r, this.cosX0 = Math.cos(this.X0), this.sinX0 = Math.sin(this.X0))
         },
@@ -38258,16 +38408,16 @@
             inverse: function(t) {
                 return ot(t, this.es, this.a, this.b)
             },
             names: ["Geocentric", "geocentric", "geocent", "Geocent"]
         },
         Ve = 0,
         He = 1,
-        Ye = 2,
-        qe = 3,
+        qe = 2,
+        Ye = 3,
         Qe = {
             h: {
                 def: 1e5,
                 num: !0
             },
             azi: {
                 def: 0,
@@ -38293,43 +38443,43 @@
             if (Object.keys(Qe).forEach(function(t) {
                     if (void 0 === this[t]) this[t] = Qe[t].def;
                     else {
                         if (Qe[t].num && isNaN(this[t])) throw new Error("Invalid parameter value, must be numeric " + t + " = " + this[t]);
                         Qe[t].num && (this[t] = parseFloat(this[t]))
                     }
                     Qe[t].degrees && (this[t] = this[t] * o)
-                }.bind(this)), Math.abs(Math.abs(this.lat0) - r) < 1e-10 ? this.mode = this.lat0 < 0 ? He : Ve : Math.abs(this.lat0) < 1e-10 ? this.mode = Ye : (this.mode = qe, this.sinph0 = Math.sin(this.lat0), this.cosph0 = Math.cos(this.lat0)), this.pn1 = this.h / this.a, this.pn1 <= 0 || this.pn1 > 1e10) throw new Error("Invalid height");
+                }.bind(this)), Math.abs(Math.abs(this.lat0) - r) < 1e-10 ? this.mode = this.lat0 < 0 ? He : Ve : Math.abs(this.lat0) < 1e-10 ? this.mode = qe : (this.mode = Ye, this.sinph0 = Math.sin(this.lat0), this.cosph0 = Math.cos(this.lat0)), this.pn1 = this.h / this.a, this.pn1 <= 0 || this.pn1 > 1e10) throw new Error("Invalid height");
             this.p = 1 + this.pn1, this.rp = 1 / this.p, this.h1 = 1 / this.pn1, this.pfact = (this.p + 1) * this.h1, this.es = 0;
             var t = this.tilt,
                 e = this.azi;
             this.cg = Math.cos(e), this.sg = Math.sin(e), this.cw = Math.cos(t), this.sw = Math.sin(t)
         },
         forward: function(t) {
             t.x -= this.long0;
             var e, n, i, r, o = Math.sin(t.y),
                 a = Math.cos(t.y),
                 s = Math.cos(t.x);
             switch (this.mode) {
-                case qe:
+                case Ye:
                     n = this.sinph0 * o + this.cosph0 * a * s;
                     break;
-                case Ye:
+                case qe:
                     n = a * s;
                     break;
                 case He:
                     n = -o;
                     break;
                 case Ve:
                     n = o
             }
             switch (e = (n = this.pn1 / (this.p - n)) * a * Math.sin(t.x), this.mode) {
-                case qe:
+                case Ye:
                     n *= this.cosph0 * o - this.sinph0 * a * s;
                     break;
-                case Ye:
+                case qe:
                     n *= o;
                     break;
                 case Ve:
                     n *= -a * s;
                     break;
                 case He:
                     n *= a * s
@@ -38344,18 +38494,18 @@
             };
             i = 1 / (this.pn1 - t.y * this.sw), e = this.pn1 * t.x * i, n = this.pn1 * t.y * this.cw * i, t.x = e * this.cg + n * this.sg, t.y = n * this.cg - e * this.sg;
             var o = Ut(t.x, t.y);
             if (Math.abs(o) < 1e-10) r.x = 0, r.y = t.y;
             else {
                 var a, s;
                 switch (s = 1 - o * o * this.pfact, s = (this.p - Math.sqrt(s)) / (this.pn1 / o + o / this.pn1), a = Math.sqrt(1 - s * s), this.mode) {
-                    case qe:
+                    case Ye:
                         r.y = Math.asin(a * this.sinph0 + t.y * s * this.cosph0 / o), t.y = (a - this.sinph0 * Math.sin(r.y)) * o, t.x *= s * this.cosph0;
                         break;
-                    case Ye:
+                    case qe:
                         r.y = Math.asin(t.y * s / o), t.y = a * o, t.x *= s;
                         break;
                     case Ve:
                         r.y = Math.asin(a), t.y = -t.y;
                         break;
                     case He:
                         r.y = -Math.asin(a)
@@ -38439,16 +38589,16 @@
                             count: a.gridNodeCount,
                             cvs: X(s)
                         }), i += 176 + 16 * a.gridNodeCount
                     }
                     return r
                 }(n, r, i)
             };
-        return q[t] = o, o
-    }, _t.transform = dt, _t.mgrs = Mt, _t.version = "__VERSION__", (Je = _t).Proj.projections.add(Bt), Je.Proj.projections.add(Wt), Je.Proj.projections.add(Vt), Je.Proj.projections.add(qt), Je.Proj.projections.add(Qt), Je.Proj.projections.add(Kt), Je.Proj.projections.add(Xt), Je.Proj.projections.add($t), Je.Proj.projections.add(te), Je.Proj.projections.add(ue), Je.Proj.projections.add(ce), Je.Proj.projections.add(pe), Je.Proj.projections.add(de), Je.Proj.projections.add(me), Je.Proj.projections.add(ge), Je.Proj.projections.add(ye), Je.Proj.projections.add(_e), Je.Proj.projections.add(ve), Je.Proj.projections.add(be), Je.Proj.projections.add(Me), Je.Proj.projections.add(we), Je.Proj.projections.add(xe), Je.Proj.projections.add(Le), Je.Proj.projections.add(Ae), Je.Proj.projections.add(Be), Je.Proj.projections.add(Ze), Je.Proj.projections.add(We), Je.Proj.projections.add(Ke), Je.Proj.projections.add(Xe);
+        return Y[t] = o, o
+    }, _t.transform = dt, _t.mgrs = Mt, _t.version = "__VERSION__", (Je = _t).Proj.projections.add(Bt), Je.Proj.projections.add(Wt), Je.Proj.projections.add(Vt), Je.Proj.projections.add(Yt), Je.Proj.projections.add(Qt), Je.Proj.projections.add(Kt), Je.Proj.projections.add(Xt), Je.Proj.projections.add($t), Je.Proj.projections.add(te), Je.Proj.projections.add(ue), Je.Proj.projections.add(ce), Je.Proj.projections.add(pe), Je.Proj.projections.add(de), Je.Proj.projections.add(me), Je.Proj.projections.add(ge), Je.Proj.projections.add(ye), Je.Proj.projections.add(_e), Je.Proj.projections.add(ve), Je.Proj.projections.add(be), Je.Proj.projections.add(Me), Je.Proj.projections.add(we), Je.Proj.projections.add(xe), Je.Proj.projections.add(Le), Je.Proj.projections.add(Ae), Je.Proj.projections.add(Be), Je.Proj.projections.add(Ze), Je.Proj.projections.add(We), Je.Proj.projections.add(Ke), Je.Proj.projections.add(Xe);
     e.default = _t
 }, function(t, e, n) {
     "use strict";
     n.d(e, "a", (function() {
         return r
     }));
     var i = n(6);
```

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/geometry_utils.py` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/metadata.json` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9653897849462365%*

 * *Differences: {"'src/lib/components/LeafletImageOverlay.react.js'": "OrderedDict([('description', "*

 * *                                                      "'图片叠加组件LeafletImageOverlay'), "*

 * *                                                      "('displayName', 'LeafletImageOverlay'), "*

 * *                                                      "('methods', []), ('props', "*

 * *                                                      "OrderedDict([('id', OrderedDict([('type', "*

 * *                                                      "Orde […]*

```diff
@@ -1706,14 +1706,133 @@
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             }
         }
     },
+    "src/lib/components/LeafletImageOverlay.react.js": {
+        "description": "\u56fe\u7247\u53e0\u52a0\u7ec4\u4ef6LeafletImageOverlay",
+        "displayName": "LeafletImageOverlay",
+        "methods": [],
+        "props": {
+            "bounds": {
+                "description": "\u5fc5\u586b\uff0c\u8bbe\u7f6e\u56fe\u7247\u53e0\u52a0\u533a\u57df\u5750\u6807\u8303\u56f4",
+                "required": true,
+                "type": {
+                    "name": "exact",
+                    "value": {
+                        "maxx": {
+                            "name": "number",
+                            "required": true
+                        },
+                        "maxy": {
+                            "name": "number",
+                            "required": true
+                        },
+                        "minx": {
+                            "name": "number",
+                            "required": true
+                        },
+                        "miny": {
+                            "name": "number",
+                            "required": true
+                        }
+                    }
+                }
+            },
+            "className": {
+                "description": "\u5f53\u524d\u56fe\u7247\u53e0\u52a0\u5c42css\u7c7b\u540d",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "id": {
+                "description": "\u7ec4\u4ef6id",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "key": {
+                "description": "\u5f3a\u5236\u5237\u65b0\u7528",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "loading_state": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "shape",
+                    "value": {
+                        "component_name": {
+                            "description": "Holds the name of the component that is loading",
+                            "name": "string",
+                            "required": false
+                        },
+                        "is_loading": {
+                            "description": "Determines if the component is loading or not",
+                            "name": "bool",
+                            "required": false
+                        },
+                        "prop_name": {
+                            "description": "Holds which property is loading",
+                            "name": "string",
+                            "required": false
+                        }
+                    }
+                }
+            },
+            "maxZoom": {
+                "description": "\u56fe\u7247\u663e\u793a\u7684\u6700\u5927\u7f29\u653e\u7ea7\u522b\uff0c\u9ed8\u8ba4\u65e0\u9650\u5236",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
+            "minZoom": {
+                "description": "\u56fe\u7247\u663e\u793a\u7684\u6700\u5c0f\u7f29\u653e\u7ea7\u522b\uff0c\u9ed8\u8ba4\u65e0\u9650\u5236",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
+            "opacity": {
+                "description": "\u56fe\u7247\u900f\u660e\u5ea6\uff0c\u53d6\u503c\u5e94\u5728`0`~`1`\u4e4b\u95f4",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
+            "setProps": {
+                "description": "Dash-assigned callback that should be called to report property changes\r\nto Dash, to make them available for callbacks.",
+                "required": false,
+                "type": {
+                    "name": "func"
+                }
+            },
+            "url": {
+                "description": "\u5fc5\u586b\uff0c\u56fe\u7247\u5730\u5740",
+                "required": true,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "zIndex": {
+                "description": "\u5f53\u524d\u56fe\u5c42z\u8f74\u5c42\u7ea7",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            }
+        }
+    },
     "src/lib/components/LeafletLayerGroup.react.js": {
         "description": "",
         "displayName": "LeafletLayerGroup",
         "methods": [],
         "props": {
             "children": {
                 "description": "",
@@ -2751,14 +2870,35 @@
             },
             "setProps": {
                 "description": "Dash-assigned callback that should be called to report property changes\r\nto Dash, to make them available for callbacks.",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
+            },
+            "syncStrategy": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "'all'"
+                },
+                "description": "\u540c\u6b65\u884c\u4e3a\u7b56\u7565\uff0c\u53ef\u9009\u9879\u6709`'all'`\u3001`'center'`\r\n\u9ed8\u8ba4\u503c\uff1a`'all'`",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "'all'"
+                        },
+                        {
+                            "computed": false,
+                            "value": "'center'"
+                        }
+                    ]
+                }
             }
         }
     },
     "src/lib/components/LeafletMarker.react.js": {
         "description": "",
         "displayName": "LeafletMarker",
         "methods": [],
@@ -4831,15 +4971,15 @@
                         }
                     ]
                 }
             }
         }
     },
     "src/lib/components/esri/EsriTiledMapLayer.react.js": {
-        "description": "",
+        "description": "ESRI tiledMapLayer\u56fe\u5c42\u7ec4\u4ef6",
         "displayName": "EsriTiledMapLayer",
         "methods": [],
         "props": {
             "debug": {
                 "defaultValue": {
                     "computed": false,
                     "value": "false"
```

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components/package-info.json` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components/package-info.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9598662207357859%*

 * *Differences: {"'dependencies'": "{'leaflet-measure': '^3.1.0'}", "'version'": "'0.1.0-rc4'"}*

```diff
@@ -9,14 +9,15 @@
         "ahooks": "^3.7.2",
         "esri-leaflet": "^3.0.12",
         "file-loader": "^6.2.0",
         "leaflet": "^1.9.4",
         "leaflet-ant-path": "^1.3.0",
         "leaflet-arrowheads": "^1.4.0",
         "leaflet-lasso": "^2.2.11",
+        "leaflet-measure": "^3.1.0",
         "leaflet-minimap": "^3.6.1",
         "leaflet-webgl-heatmap": "^0.2.7",
         "leaflet.heat": "^0.2.0",
         "leaflet.motion": "^0.3.2",
         "leaflet.vectorgrid": "^1.3.0",
         "lodash": "^4.17.21",
         "proj4leaflet": "^1.0.2",
@@ -73,9 +74,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_leaflet_components -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.1.0-rc3"
+    "version": "0.1.0-rc4"
 }
```

### Comparing `feffery_leaflet_components-0.1.0rc3/feffery_leaflet_components.egg-info/SOURCES.txt` & `feffery_leaflet_components-0.1.0rc4/feffery_leaflet_components.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 feffery_leaflet_components/LeafletDomWrapper.py
 feffery_leaflet_components/LeafletExport.py
 feffery_leaflet_components/LeafletFeatureGroup.py
 feffery_leaflet_components/LeafletFlowLayer.py
 feffery_leaflet_components/LeafletFullscreenControl.py
 feffery_leaflet_components/LeafletGeoJSON.py
 feffery_leaflet_components/LeafletHeatMap.py
+feffery_leaflet_components/LeafletImageOverlay.py
 feffery_leaflet_components/LeafletLayerGroup.py
 feffery_leaflet_components/LeafletMap.py
 feffery_leaflet_components/LeafletMapAction.py
 feffery_leaflet_components/LeafletMapListener.py
 feffery_leaflet_components/LeafletMapProvider.py
 feffery_leaflet_components/LeafletMapSync.py
 feffery_leaflet_components/LeafletMarker.py
```

### Comparing `feffery_leaflet_components-0.1.0rc3/package.json` & `feffery_leaflet_components-0.1.0rc4/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9598662207357859%*

 * *Differences: {"'dependencies'": "{'leaflet-measure': '^3.1.0'}", "'version'": "'0.1.0-rc4'"}*

```diff
@@ -9,14 +9,15 @@
         "ahooks": "^3.7.2",
         "esri-leaflet": "^3.0.12",
         "file-loader": "^6.2.0",
         "leaflet": "^1.9.4",
         "leaflet-ant-path": "^1.3.0",
         "leaflet-arrowheads": "^1.4.0",
         "leaflet-lasso": "^2.2.11",
+        "leaflet-measure": "^3.1.0",
         "leaflet-minimap": "^3.6.1",
         "leaflet-webgl-heatmap": "^0.2.7",
         "leaflet.heat": "^0.2.0",
         "leaflet.motion": "^0.3.2",
         "leaflet.vectorgrid": "^1.3.0",
         "lodash": "^4.17.21",
         "proj4leaflet": "^1.0.2",
@@ -73,9 +74,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_leaflet_components -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.1.0-rc3"
+    "version": "0.1.0-rc4"
 }
```

### Comparing `feffery_leaflet_components-0.1.0rc3/setup.py` & `feffery_leaflet_components-0.1.0rc4/setup.py`

 * *Files identical despite different names*

