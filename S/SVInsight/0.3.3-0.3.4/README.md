# Comparing `tmp/svinsight-0.3.3.tar.gz` & `tmp/svinsight-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svinsight-0.3.3.tar", last modified: Thu Apr 25 21:36:09 2024, max compression
+gzip compressed data, was "svinsight-0.3.4.tar", last modified: Mon Apr 29 14:19:27 2024, max compression
```

## Comparing `svinsight-0.3.3.tar` & `svinsight-0.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:36:09.745078 svinsight-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-25 21:36:04.000000 svinsight-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 21:36:09.745078 svinsight-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-25 21:36:04.000000 svinsight-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:36:09.745078 svinsight-0.3.3/SVInsight/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 21:36:04.000000 svinsight-0.3.3/SVInsight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-25 21:36:04.000000 svinsight-0.3.3/SVInsight/census_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    76938 2024-04-25 21:36:04.000000 svinsight-0.3.3/SVInsight/svi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:36:09.745078 svinsight-0.3.3/SVInsight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 21:36:09.000000 svinsight-0.3.3/SVInsight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 21:36:09.000000 svinsight-0.3.3/SVInsight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 21:36:09.000000 svinsight-0.3.3/SVInsight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 21:36:09.000000 svinsight-0.3.3/SVInsight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-25 21:36:05.000000 svinsight-0.3.3/long_desc.md
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-25 21:36:05.000000 svinsight-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 21:36:09.745078 svinsight-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 21:36:09.745078 svinsight-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-25 21:36:05.000000 svinsight-0.3.3/tests/test_svinsight.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:19:27.220581 svinsight-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-29 14:19:22.000000 svinsight-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-29 14:19:27.220581 svinsight-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-29 14:19:22.000000 svinsight-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:19:27.220581 svinsight-0.3.4/SVInsight/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-29 14:19:22.000000 svinsight-0.3.4/SVInsight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-29 14:19:22.000000 svinsight-0.3.4/SVInsight/census_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76953 2024-04-29 14:19:22.000000 svinsight-0.3.4/SVInsight/svi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:19:27.220581 svinsight-0.3.4/SVInsight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-29 14:19:27.000000 svinsight-0.3.4/SVInsight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-29 14:19:27.000000 svinsight-0.3.4/SVInsight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:19:27.000000 svinsight-0.3.4/SVInsight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 14:19:27.000000 svinsight-0.3.4/SVInsight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 14:19:22.000000 svinsight-0.3.4/long_desc.md
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-29 14:19:22.000000 svinsight-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:19:27.224581 svinsight-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:19:27.220581 svinsight-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-29 14:19:22.000000 svinsight-0.3.4/tests/test_svinsight.py
```

### Comparing `svinsight-0.3.3/LICENSE` & `svinsight-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `svinsight-0.3.3/README.md` & `svinsight-0.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SVInsight: Social Vulnerability Index Creation 
 ![pages-build-deployment](https://github.com/mdp0023/SVInsight/actions/workflows/pages/pages-build-deployment/badge.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/svinsight)
 ![PyPI](https://img.shields.io/pypi/v/svinsight)
 
-*SVInsight* is a python package for calculating an exploratory social vulnerability index. This package calculates SVI using two methods: (1) an iterative factor analysis method and (2) a rank method, both of which have been heavily utilized in scholarly research. This package automates the creation and comparisons of indices using U.S. American Community Survey 5-Year Data (ACS5) at the block group or tract level. Users can customize which social, demographic, and economic variables are included in their own custom indices.
+*SVInsight* is a python package for calculating an exploratory social vulnerability index. This package calculates SVI using two methods: (1) an iterative factor analysis method and (2) a rank method, both of which have been heavily utilized in scholarly research. This package automates the creation and comparison of indices using U.S. American Community Survey 5-Year Data (ACS5) at the block group or tract level. Users can customize which social, demographic, and economic variables are included in their own custom indices.
 
 This package is a tool to efficiently calculate an exploratory estimate of social vulnerability for a given region. Social vulnerability is an incredibly complex and constantly evolving concept, and researchers, practitioners, and users of this software should always consult relevant peer-reviewed literature and local experts to validate findings.
 
 For user guides, examples, and a more indepth discussion of social vulnerability indices, refer to the [documentation](https://mdp0023.github.io/SVInsight/).
```

### Comparing `svinsight-0.3.3/SVInsight/census_variables.py` & `svinsight-0.3.4/SVInsight/census_variables.py`

 * *Files identical despite different names*

### Comparing `svinsight-0.3.3/SVInsight/svi.py` & `svinsight-0.3.4/SVInsight/svi.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,15 @@
             elif boundary == 'tract':
                 shapefile['tract_fips'] = shapefile['GEOID']
                 # merge geopandas shapefile with data_df shapefile
                 data_df = data_df.merge(shapefile, on='tract_fips', how='left')
             # convert data_df to geopandas
             data_df = gpd.GeoDataFrame(data_df, geometry=data_df['geometry'])
             # reset index of geodataframe
-            data_df['index'] = data_df['GEOID'].astype(int)
+            data_df['index'] = data_df['GEOID'].astype(np.int64)
             data_df = data_df.set_index('index')
 
             # Fill in missing holes
             data_df = self._fill_holes(data_df, boundary, self.geoids, self.api_key, year, interpolate, verbose)
 
             # Save as csv and shapefile
             data_df.to_csv(os.path.join(self.data, f"{self.project_name}_{year}_{boundary}_rawdata.csv"))
@@ -460,15 +460,15 @@
                 # merge geopandas shapefile with data_df shapefile
                 data_df = data_df.merge(shapefile, on='tract_fips', how='right', suffixes=('', '_y'))
             data_df.drop(data_df.filter(regex='_y$').columns, axis=1, inplace=True)
 
             # convert data_df to geopandas
             data_df = gpd.GeoDataFrame(data_df, geometry=data_df['geometry'])
             # reset index of geodataframe
-            data_df['index'] = data_df['GEOID'].astype(int)
+            data_df['index'] = data_df['GEOID'].astype(np.int64)
             data_df = data_df.set_index('index')
             # Fill in missing holes
             data_df = self._fill_holes(data_df, boundary, self.geoids, self.api_key, year, interpolate=True, verbose=False)
 
             data_df.to_csv(os.path.join(self.data, f"{self.project_name}_{year}_{boundary}_rawdata.csv"))
             data_df.to_file(os.path.join(self.data, f"{self.project_name}_{year}_{boundary}_rawdata.gpkg"))
 
@@ -1328,15 +1328,15 @@
         Returns:
             tuple: A tuple containing two lists - `miss_vals` and `unique_missing_vals`.
                 - `miss_vals` (list): A list of missing values in the DataFrame. First value is GEOID of hole, and second value is variable.
                 - `unique_missing_vals` (list): A list of unique missing values found in the DataFrame.
 
         """
         # Fill in missing holes
-        miss_vals = data_df.where(data_df.map(lambda x: isinstance(x, (int, float)) and x < 0)).stack().index
+        miss_vals = data_df.where(data_df.map(lambda x: isinstance(x, (np.int64, float)) and x < 0)).stack().index
         # Find the unique missing_vars
         unique_missing_vals = []
         for miss_val in miss_vals:
             if miss_val[1] not in unique_missing_vals:
                 unique_missing_vals.append(miss_val[1])  
 
         return miss_vals, unique_missing_vals
```

### Comparing `svinsight-0.3.3/pyproject.toml` & `svinsight-0.3.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SVInsight"
-version = "0.3.3"
+version = "0.3.4"
 description = "Create social vulnerabilty index"
 readme = "long_desc.md"
 license = { file = "LICENSE.txt" }
+requires-python = ">=3.9"
 
 
 [options]
 python_requires = ">=3.9"
 install_requires = [
     "census",
     "factor_analyzer",
```

### Comparing `svinsight-0.3.3/tests/test_svinsight.py` & `svinsight-0.3.4/tests/test_svinsight.py`

 * *Files identical despite different names*

