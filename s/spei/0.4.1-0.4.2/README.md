# Comparing `tmp/spei-0.4.1.tar.gz` & `tmp/spei-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spei-0.4.1.tar", last modified: Thu Mar 28 19:01:03 2024, max compression
+gzip compressed data, was "spei-0.4.2.tar", last modified: Mon Apr 29 21:01:43 2024, max compression
```

## Comparing `spei-0.4.1.tar` & `spei-0.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:01:03.151187 spei-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-28 19:00:52.000000 spei-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-03-28 19:01:03.151187 spei-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-03-28 19:00:52.000000 spei-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-03-28 19:00:52.000000 spei-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 19:01:03.151187 spei-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:01:03.147187 spei-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:01:03.147187 spei-0.4.1/src/spei/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-28 19:00:52.000000 spei-0.4.1/src/spei/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-28 19:00:52.000000 spei-0.4.1/src/spei/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-28 19:00:52.000000 spei-0.4.1/src/spei/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-03-28 19:00:52.000000 spei-0.4.1/src/spei/climdex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-03-28 19:00:52.000000 spei-0.4.1/src/spei/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    14767 2024-03-28 19:00:52.000000 spei-0.4.1/src/spei/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 19:00:52.000000 spei-0.4.1/src/spei/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13533 2024-03-28 19:00:52.000000 spei-0.4.1/src/spei/si.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-03-28 19:00:52.000000 spei-0.4.1/src/spei/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:01:03.151187 spei-0.4.1/src/spei.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-03-28 19:01:03.000000 spei-0.4.1/src/spei.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-28 19:01:03.000000 spei-0.4.1/src/spei.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 19:01:03.000000 spei-0.4.1/src/spei.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-28 19:01:03.000000 spei-0.4.1/src/spei.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-28 19:01:03.000000 spei-0.4.1/src/spei.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 19:01:03.147187 spei-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-28 19:00:52.000000 spei-0.4.1/tests/test_climdex.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-28 19:00:52.000000 spei-0.4.1/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-28 19:00:52.000000 spei-0.4.1/tests/test_si.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-28 19:00:52.000000 spei-0.4.1/tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-28 19:00:52.000000 spei-0.4.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:01:43.454634 spei-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 21:01:33.000000 spei-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-29 21:01:43.454634 spei-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-04-29 21:01:33.000000 spei-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-29 21:01:33.000000 spei-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 21:01:43.454634 spei-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:01:43.446634 spei-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:01:43.450634 spei-0.4.2/src/spei/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-29 21:01:33.000000 spei-0.4.2/src/spei/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-29 21:01:33.000000 spei-0.4.2/src/spei/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-29 21:01:33.000000 spei-0.4.2/src/spei/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-29 21:01:33.000000 spei-0.4.2/src/spei/climdex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-29 21:01:33.000000 spei-0.4.2/src/spei/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14767 2024-04-29 21:01:33.000000 spei-0.4.2/src/spei/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 21:01:33.000000 spei-0.4.2/src/spei/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17064 2024-04-29 21:01:33.000000 spei-0.4.2/src/spei/si.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-29 21:01:33.000000 spei-0.4.2/src/spei/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:01:43.450634 spei-0.4.2/src/spei.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-29 21:01:43.000000 spei-0.4.2/src/spei.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-29 21:01:43.000000 spei-0.4.2/src/spei.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 21:01:43.000000 spei-0.4.2/src/spei.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-29 21:01:43.000000 spei-0.4.2/src/spei.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 21:01:43.000000 spei-0.4.2/src/spei.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:01:43.450634 spei-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-29 21:01:33.000000 spei-0.4.2/tests/test_climdex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-29 21:01:33.000000 spei-0.4.2/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-29 21:01:33.000000 spei-0.4.2/tests/test_si.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-29 21:01:33.000000 spei-0.4.2/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-29 21:01:33.000000 spei-0.4.2/tests/test_version.py
```

### Comparing `spei-0.4.1/LICENSE` & `spei-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spei-0.4.1/PKG-INFO` & `spei-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spei
-Version: 0.4.1
+Version: 0.4.2
 Summary: A simple Python package to calculate drought indices for time series such as the SPI, SPEI and SGI.
 Author-email: Martin Vonk <vonk.mart@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Martin Vonk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `spei-0.4.1/README.md` & `spei-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `spei-0.4.1/pyproject.toml` & `spei-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spei-0.4.1/src/spei/climdex.py` & `spei-0.4.2/src/spei/climdex.py`

 * *Files identical despite different names*

### Comparing `spei-0.4.1/src/spei/dist.py` & `spei-0.4.2/src/spei/dist.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,30 +98,30 @@
             *pars, loc, scale = fit_tuple
         return pars, loc, scale
 
     def cdf(self) -> Series:
         """Compute cumulative density function of a Scipy Continuous Distribution"""
         if self.pars is not None:
             cdf = self.dist.cdf(
-                self.data.values, self.pars, loc=self.loc, scale=self.scale
+                self.data.values, *self.pars, loc=self.loc, scale=self.scale
             )
         else:
             cdf = self.dist.cdf(self.data.values, loc=self.loc, scale=self.scale)
 
         if self.prob_zero:
             cdf = self.p0 + (1 - self.p0) * cdf
             cdf[self.data == 0.0] = self.p0
 
         return Series(cdf, index=self.data.index, dtype=float)
 
     def pdf(self) -> Series:
         data_pdf = self.data.sort_values()
         if self.pars is not None:
             pdf = self.dist.pdf(
-                data_pdf.values, self.pars, loc=self.loc, scale=self.scale
+                data_pdf.values, *self.pars, loc=self.loc, scale=self.scale
             )
         else:
             pdf = self.dist.pdf(data_pdf.values, loc=self.loc, scale=self.scale)
 
         # TODO: check what to do if prob_zero
 
         return Series(pdf, index=data_pdf.index, dtype=float)
```

### Comparing `spei-0.4.1/src/spei/plot.py` & `spei-0.4.2/src/spei/plot.py`

 * *Files identical despite different names*

### Comparing `spei-0.4.1/src/spei/si.py` & `spei-0.4.2/src/spei/si.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,14 +26,18 @@
     cumulative density function.
 
     Parameters
     ----------
     series: pandas.Series
         Pandas time series of the groundwater levels. Time series index
         should be a pandas DatetimeIndex.
+    fit_freq : str, optional, default=None
+        Frequency for fitting the distribution. Default is None in which case
+        the frequency of the series is inferred. If this fails a monthly
+        frequency is used.
 
     Returns
     -------
     pandas.Series
 
     References
     ----------
@@ -71,17 +75,34 @@
         Pandas time series of the precipitation. Time series index
         should be a pandas DatetimeIndex.
     dist: scipy.stats.rv_continuous
         Can be any continuous distribution from the scipy.stats library.
         However, for the SPI generally the Gamma probability density
         function is recommended. Other appropriate choices could be the
         lognormal, log-logistic (fisk) or PearsonIII distribution.
-    prob_zero: bool
-        Option to correct the distribution if x=0 is not in probability
-        density function. E.g. the case with the Gamma distriubtion.
+    timescale : int, optional, default=0
+        Size of the moving window over which the series is summed. If zero, no
+        summation is performed over the time series. If the time series
+        frequency is daily, then one would provide timescale=30 for SI1,
+        timescale=90 for SI3, timescale=180 for SI6 etc.
+    fit_freq : str, optional, default=None
+        Frequency for fitting the distribution. Default is None in which case
+        the frequency of the series is inferred. If this fails a monthly
+        frequency is used.
+    fit_window : int, optional, default=0
+        Window size for fitting data in fit_freq frequency's unit. Default is
+        zero in which case only data within the fit_freq is considered. If
+        larger than zero data data within the window is used to fit the
+        distribution for the series. fit_window must be a odd number larger
+        than 3 when used.
+    prob_zero : bool, default=True
+        Option to correct the distribution if x=0 is not in probability density
+        function. E.g. the case with the Gamma distriubtion. If True, the
+        probability of zero values in the series is calculated by the
+        occurence.
 
     Returns
     -------
     pandas.Series
 
     References
     ----------
@@ -120,14 +141,32 @@
         Pandas time series of the precipitation. Time series index
         should be a pandas DatetimeIndex.
     dist: scipy.stats.rv_continuous
         Can be any continuous distribution from the scipy.stats library.
         However, for the SPEI generally the log-logistic (fisk) probability
         density function is recommended. Other appropriate choices could be
         the lognormal or PearsonIII distribution.
+    timescale : int, optional, default=0
+        Size of the moving window over which the series is summed. If zero, no
+        summation is performed over the time series. If the time series
+        frequency is daily, then one would provide timescale=30 for SI1,
+        timescale=90 for SI3, timescale=180 for SI6 etc.
+    fit_freq : str, optional, default=None
+        Frequency for fitting the distribution. Default is None in which case
+        the frequency of the series is inferred. If this fails a monthly
+        frequency is used.
+    fit_window : int, optional, default=0
+        Window size for fitting data in fit_freq frequency's unit. Default is
+        zero in which case only data within the fit_freq is considered. If
+        larger than zero data data within the window is used to fit the
+        distribution for the series. fit_window must be a odd number larger
+        than 3 when used.
+    prob_zero : bool, default=False
+        Flag indicating whether the probability of zero values in the series is
+        calculated by the occurence.
 
     Returns
     -------
     pandas.Series
 
     References
     ----------
@@ -166,14 +205,32 @@
         Pandas time series of the precipitation. Time series index
         should be a pandas DatetimeIndex.
     dist: scipy.stats.rv_continuous
         Can be any continuous distribution from the scipy.stats library.
         However, for the SSFI generally the gamma probability density
         function is recommended. Other appropriate choices could be the
         normal, lognormal, pearsonIII, GEV or  Gen-Logistic distribution.
+    timescale : int, optional, default=0
+        Size of the moving window over which the series is summed. If zero, no
+        summation is performed over the time series. If the time series
+        frequency is daily, then one would provide timescale=30 for SI1,
+        timescale=90 for SI3, timescale=180 for SI6 etc.
+    fit_freq : str, optional, default=None
+        Frequency for fitting the distribution. Default is None in which case
+        the frequency of the series is inferred. If this fails a monthly
+        frequency is used.
+    fit_window : int, optional, default=0
+        Window size for fitting data in fit_freq frequency's unit. Default is
+        zero in which case only data within the fit_freq is considered. If
+        larger than zero data data within the window is used to fit the
+        distribution for the series. fit_window must be a odd number larger
+        than 3 when used.
+    prob_zero : bool, default=False
+        Flag indicating whether the probability of zero values in the series is
+        calculated by the occurence.
 
     Returns
     -------
     pandas.Series
 
     References
     ----------
@@ -203,17 +260,18 @@
     Parameters
     ----------
     series : Series
         The input time series data.
     dist : ContinuousDist
         The SciPy continuous distribution associated with the data.
     timescale : int, optional, default=0
-        Rolling window timescale in days over which the series is summed. For
-        SI1 the user would provide timescale=30, for SI3: timescale=90, SI6:
-        timescale=180 etc.
+        Size of the moving window over which the series is summed. If zero, no
+        summation is performed over the time series. If the time series
+        frequency is daily, then one would provide timescale=30 for SI1,
+        timescale=90 for SI3, timescale=180 for SI6 etc.
     fit_freq : str, optional, default=None
         Frequency for fitting the distribution. Default is None in which case
         the frequency of the series is inferred. If this fails a monthly
         frequency is used.
     fit_window : int, optional, default=0
         Window size for fitting data in fit_freq frequency's unit. Default is
         zero in which case only data within the fit_freq is considered. If
@@ -254,15 +312,15 @@
         Post initializes the SI class and performs necessary data
         preprocessing and validation.
         """
         self.series = validate_series(self.series)
 
         if self.timescale > 0:
             self.series = (
-                self.series.rolling(f"{self.timescale}D", min_periods=self.timescale)
+                self.series.rolling(self.timescale, min_periods=self.timescale)
                 .sum()
                 .dropna()
                 .copy()
             )
 
         if self.fit_freq is None:
             self.fit_freq = infer_frequency(self.series.index)
```

### Comparing `spei-0.4.1/src/spei/utils.py` & `spei-0.4.2/src/spei/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     inf_freq = infer_freq(index)
 
     if inf_freq is None:
         logging.info(
             "Could not infer frequency from index, using monthly frequency instead"
         )
-        inf_freq = "ME" if pd_version >= "2.1.0" else "M"
+        inf_freq = "ME" if pd_version >= "2.2.0" else "M"
     else:
         logging.info(f"Inferred frequency '{inf_freq}' from index")
 
     if "W-" in inf_freq:
         logging.info(f"Converted frequncy weekly '{inf_freq}' to 'W'")
         inf_freq = "W"
 
@@ -77,15 +77,15 @@
 
 def group_yearly_df(series: Series) -> DataFrame:
     """Group series in a DataFrame with date (in the year 2000) as index and
     year as columns.
     """
     strfstr: str = "%m-%d %H:%M:%S"
     grs = {}
-    freq = "YE" if pd_version >= "2.1.0" else "Y"
+    freq = "YE" if pd_version >= "2.2.0" else "Y"
     for year_timestamp, gry in series.groupby(Grouper(freq=freq)):
         index = validate_index(gry.index)
         gry.index = to_datetime(
             "2000-" + index.strftime(strfstr), format="%Y-" + strfstr
         )
         year = getattr(year_timestamp, "year")  # type: str
         grs[year] = gry
```

### Comparing `spei-0.4.1/src/spei.egg-info/PKG-INFO` & `spei-0.4.2/src/spei.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spei
-Version: 0.4.1
+Version: 0.4.2
 Summary: A simple Python package to calculate drought indices for time series such as the SPI, SPEI and SGI.
 Author-email: Martin Vonk <vonk.mart@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Martin Vonk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `spei-0.4.1/tests/test_climdex.py` & `spei-0.4.2/tests/test_climdex.py`

 * *Files identical despite different names*

### Comparing `spei-0.4.1/tests/test_si.py` & `spei-0.4.2/tests/test_si.py`

 * *Files identical despite different names*

### Comparing `spei-0.4.1/tests/test_validate.py` & `spei-0.4.2/tests/test_validate.py`

 * *Files identical despite different names*

