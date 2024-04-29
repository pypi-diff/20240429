# Comparing `tmp/wsat-0.1.1.tar.gz` & `tmp/wsat-0.1.2.tar.gz`

## Comparing `wsat-0.1.1.tar` & `wsat-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wsat-0.1.1/WSAT/__init__.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 wsat-0.1.1/WSAT/wsat_extraplots.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 wsat-0.1.1/WSAT/wsat_loadwind.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 wsat-0.1.1/WSAT/wsat_windplot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wsat-0.1.1/.gitignore
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 wsat-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 wsat-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wsat-0.1.2/WSAT/__init__.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 wsat-0.1.2/WSAT/wsat_extraplots.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 wsat-0.1.2/WSAT/wsat_loadwind.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 wsat-0.1.2/WSAT/wsat_windplot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wsat-0.1.2/.gitignore
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 wsat-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 wsat-0.1.2/PKG-INFO
```

### Comparing `wsat-0.1.1/WSAT/wsat_extraplots.py` & `wsat-0.1.2/WSAT/wsat_extraplots.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,19 +29,20 @@
     outlier_mask = np.ma.masked_where(wind_speed <  30, wind_speed).mask
     # Create valid mask
     valid_mask = np.logical_not(outlier_mask)
     # Apply valid mask to the original scene
     valid_ws = np.ma.masked_where(valid_mask, wind_speed)
     sar_scene = np.nansum(valid_ws,0) # calculating SAR scenes
     plt.pcolor(x_lon,y_lat,sar_scene,cmap = "viridis")
-    plt.colorbar()
+    cbar = plt.colorbar()
+    cbar.set_label('Number of SAR scenes')
     plt.xlabel('Longitude')
     plt.ylabel('Latitude')
 
     # Removing NaN values from wind speed array
     w_speed = wind_speed[~np.isnan(wind_speed)]
     # Removing NaN values from wind direction array
     w_direction = wind_dir[~np.isnan(wind_dir)]
     ax_rose = WindroseAxes.from_ax()
     ax_rose.bar(w_direction, w_speed,normed=True, bins=np.arange(0, 30, 2.5))
-    ax_rose.set_legend()
+    ax_rose.set_legend(units = 'm/s')
     plt.show()
```

### Comparing `wsat-0.1.1/WSAT/wsat_loadwind.py` & `wsat-0.1.2/WSAT/wsat_loadwind.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Parameters:
         file_paths (str): Path to the directory containing NetCDF files.
         lat_params (tuple): Tuple containing (lat_name, lat_range).
         lon_params (tuple): Tuple containing (lon_name, lon_range).
         wind_names (tuple): Tuple containing (wind_speed_name, wind_direction_name).
 
     Returns:
-        wind_data (dict): Dicti½onary containing wind data with lat, lon.
+        wind_data (dict): Dictionary containing wind data with lat, lon.
     """
     lat_name, lat_range = lat_params
     lon_name, lon_range = lon_params
     ws_name, wd_name = wind_names
     wind_data = {'latitude': [], 'longitude': [], 'speed': [], 'direction': []}
 
     # Load latitude and longitude
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `wsat-0.1.1/WSAT/wsat_windplot.py` & `wsat-0.1.2/WSAT/wsat_windplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import warnings
 import numpy as np
 import matplotlib.pyplot as plt
 from mpl_toolkits.basemap import Basemap
 
 def plot_wind_map(wind_data):
     """
-    Plot wind map using wind data.
+    Plot wind resource map using wind data.
 
     Parameters:
         wind_data (dict): Dictionary containing wind data with lat, lon.
 
     Returns:
         None
     """
@@ -37,19 +37,19 @@
     plt.figure(figsize=(10, 8))
     b_map = Basemap(projection='cyl',llcrnrlon=np.min(lon),llcrnrlat=np.min(lat),
                     urcrnrlon=np.max(lon),urcrnrlat=np.max(lat),epsg=4326,resolution='f')
     b_map.shadedrelief()
     b_map.drawcoastlines()
     b_map.drawcountries(linewidth=1, linestyle='solid', color='k')
     plt.title("Shaded relief image as background map", fontsize=18)
-    plt.pcolor(x_lon, y_lat, mean_wind_speed, cmap='plasma')
+    plt.pcolor(x_lon, y_lat, mean_wind_speed, cmap='viridis')
     plt.gca().tick_params(labelsize=18)
     plt.clim(0, 20)  # Colormap limit
     plt.colorbar(label='Wind speed m/s')
-    step = 15
+    step = 17
     plt.quiver(x_lon[::step, ::step], y_lat[::step, ::step],
                mean_u[::step, ::step], mean_v[::step, ::step], mean_wind_speed[::step, ::step],
                cmap="gist_gray", units='xy')
     plt.title('Wind map with Basemap', fontsize=18)
     plt.xlabel('Longitude', fontsize=14)
     plt.ylabel('Latitude', fontsize=14)
     plt.show()
```

### Comparing `wsat-0.1.1/pyproject.toml` & `wsat-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 build-backend = "hatchling.build"
 [tool.hatch.build.targets.wheel]
 packages = ["WSAT"]
 # Information on the package
 [project]
 name = "WSAT"
 description = "A data visualization package"
-version = "0.1.1"   
+version = "0.1.2    "   
 authors = [
     { name = "S.F.K", email = "Simonfogh@hotmail.com" }
 ]
 #dependencies = #["os",
 #    "Warnings",
 #    "numpy",
 #    "Matplotlib",
```

