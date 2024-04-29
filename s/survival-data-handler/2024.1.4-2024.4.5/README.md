# Comparing `tmp/survival_data_handler-2024.1.4.tar.gz` & `tmp/survival_data_handler-2024.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survival_data_handler-2024.1.4.tar", last modified: Fri Apr 26 17:54:29 2024, max compression
+gzip compressed data, was "survival_data_handler-2024.4.5.tar", last modified: Mon Apr 29 13:26:56 2024, max compression
```

## Comparing `survival_data_handler-2024.1.4.tar` & `survival_data_handler-2024.4.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:29.381084 survival_data_handler-2024.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-26 17:54:29.381084 survival_data_handler-2024.1.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2108 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 17:54:29.381084 survival_data_handler-2024.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:29.377084 survival_data_handler-2024.1.4/survival_data_handler/
--rwxr-xr-x   0 runner    (1001) docker     (127)      762 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/survival_data_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/survival_data_handler/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16777 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/survival_data_handler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/survival_data_handler/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/survival_data_handler/plotting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5863 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/survival_data_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:29.381084 survival_data_handler-2024.1.4/survival_data_handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-26 17:54:29.000000 survival_data_handler-2024.1.4/survival_data_handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-26 17:54:29.000000 survival_data_handler-2024.1.4/survival_data_handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:54:29.000000 survival_data_handler-2024.1.4/survival_data_handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-26 17:54:29.000000 survival_data_handler-2024.1.4/survival_data_handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 17:54:29.000000 survival_data_handler-2024.1.4/survival_data_handler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:54:29.381084 survival_data_handler-2024.1.4/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5496 2024-04-26 17:54:20.000000 survival_data_handler-2024.1.4/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:56.478223 survival_data_handler-2024.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-29 13:26:51.000000 survival_data_handler-2024.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-29 13:26:56.478223 survival_data_handler-2024.4.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2108 2024-04-29 13:26:51.000000 survival_data_handler-2024.4.5/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-29 13:26:51.000000 survival_data_handler-2024.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 13:26:51.000000 survival_data_handler-2024.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:26:56.478223 survival_data_handler-2024.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:56.474223 survival_data_handler-2024.4.5/survival_data_handler/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      762 2024-04-29 13:26:51.000000 survival_data_handler-2024.4.5/survival_data_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-29 13:26:51.000000 survival_data_handler-2024.4.5/survival_data_handler/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16908 2024-04-29 13:26:51.000000 survival_data_handler-2024.4.5/survival_data_handler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-29 13:26:51.000000 survival_data_handler-2024.4.5/survival_data_handler/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-29 13:26:51.000000 survival_data_handler-2024.4.5/survival_data_handler/plotting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6358 2024-04-29 13:26:51.000000 survival_data_handler-2024.4.5/survival_data_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:56.478223 survival_data_handler-2024.4.5/survival_data_handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-29 13:26:56.000000 survival_data_handler-2024.4.5/survival_data_handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-29 13:26:56.000000 survival_data_handler-2024.4.5/survival_data_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:26:56.000000 survival_data_handler-2024.4.5/survival_data_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-29 13:26:56.000000 survival_data_handler-2024.4.5/survival_data_handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 13:26:56.000000 survival_data_handler-2024.4.5/survival_data_handler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:56.478223 survival_data_handler-2024.4.5/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5805 2024-04-29 13:26:51.000000 survival_data_handler-2024.4.5/test/test_main.py
```

### Comparing `survival_data_handler-2024.1.4/LICENSE` & `survival_data_handler-2024.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.1.4/PKG-INFO` & `survival_data_handler-2024.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survival_data_handler
-Version: 2024.1.4
+Version: 2024.4.5
 Author-email: Vincent Laurent <vlaurent@eurobios.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3
 Requires-Dist: seaborn
 Requires-Dist: numba
 Requires-Dist: scipy
```

### Comparing `survival_data_handler-2024.1.4/README.md` & `survival_data_handler-2024.4.5/README.md`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.1.4/survival_data_handler/__init__.py` & `survival_data_handler-2024.4.5/survival_data_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.1.4/survival_data_handler/base.py` & `survival_data_handler-2024.4.5/survival_data_handler/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,27 +24,35 @@
     @property
     def survival_function(self):
         self.__curve[self.__curve > 1] = 1
         self.__curve[self.__curve < 0] = 0
         return self.__curve
 
     @property
+    def density_function(self):
+        return - self.survival_function.derivative()
+
+    @property
     def hazard_function(self):
-        return self.survival_function.derivative()
+        return self.density_function / self.survival_function
 
     @property
     def cumulative_hazard_function(self):
         return - self.survival_function.log()
 
     @property
     def residual_life(self):
         ret = residual_life(self.survival_function)
         ret.columns = self.survival_function.columns
         return TimeCurveData(ret)
 
+    @property
+    def lifetime_distribution_function(self):
+        return 1 - self.survival_function
+
 
 class TimeCurve:
 
     def __interpolator(self):
         pass
 
 
@@ -72,35 +80,41 @@
     def log(self):
         return TimeCurveData(np.log(self))
 
     def exp(self):
         return TimeCurveData(np.exp(self))
 
     def __truediv__(self, other):
-        return TimeCurveData(pd.DataFrame(self.values / other.values, columns=self.columns, index=self.index),
+        return TimeCurveData(pd.DataFrame(self.values / self.__other(other), columns=self.columns, index=self.index),
                              unit=self.unit, n_unit=self.n_unit)
 
     def __add__(self, other):
-        return TimeCurveData(pd.DataFrame(self.values + other.values, columns=self.columns, index=self.index),
+        return TimeCurveData(pd.DataFrame(self.values + self.__other(other), columns=self.columns, index=self.index),
                              unit=self.unit, n_unit=self.n_unit)
 
     def __sub__(self, other):
-        return TimeCurveData(pd.DataFrame(self.values - other.values, columns=self.columns, index=self.index),
+        return TimeCurveData(pd.DataFrame(self.values - self.__other(other), columns=self.columns, index=self.index),
                              unit=self.unit, n_unit=self.n_unit)
 
     def __neg__(self):
         return TimeCurveData(pd.DataFrame(-self.values, index=self.index, columns=self.columns), unit=self.unit,
                              n_unit=self.n_unit)
 
     @property
     def interpolation(self) -> dict:
         if not hasattr(self, "__interpolation"):
             self.__interpolator()
         return self.__interpolation
 
+    def __other(self, other):
+        if hasattr(other, "values"):
+            return other.values
+        else:
+            return other
+
 
 class TimeCurveInterpolation(TimeCurve):
 
     def __init__(
             self,
             interpolation: dict,
             birth, index: pd.Series,
```

### Comparing `survival_data_handler-2024.1.4/survival_data_handler/main.py` & `survival_data_handler-2024.4.5/survival_data_handler/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # ======================================================================================================================
 # AESTHETICS
 cmap = sns.color_palette('rainbow', as_cmap=True)
 event_censored_color = cmap(0.1)
 event_observed_color = cmap(0.95)
 
 
-class Lifespan:
+class Lifespan(SurvivalCurves):
     __index = "origin_index"
 
     def __init__(self, ageing_curves: pd.DataFrame, index: iter, age: iter, birth: iter, window: tuple,
                  default_precision="float"):
 
         self.__curves = TimeCurveData(ageing_curves.__deepcopy__())
         self.df_idx = pd.DataFrame(dict(age=age, birth=birth, index=index))
@@ -55,14 +55,15 @@
                                  on=["birth", "index"], suffixes=("_u", ""))
 
         self._corresp = self._corresp.drop(columns=c)
         self.confusion_matrix_threshold = np.nan
         self.__computed = []
         self.__supervised = False
         self.__interpolator = {}
+        super().__init__(self.survival_function)
 
     def __check_args(self):
 
         if hasattr(self.curves.columns, "dt"):
             ValueError("curves index must have dt property")
 
     @property
@@ -83,14 +84,15 @@
         ret = self.__getattribute__(on)
         if not get_supervision:
             return ret, None, None, None
         else:
             index = [i for i in ret.index if i in self.event.index]
             entry = self.entry if self.entry is None else self.entry.loc[index]
             return ret.loc[index], self.event.loc[index], self.durations.loc[index], entry
+
     def _decompose_unique(self, data, get_supervision=False):
         ret = pd.merge(self._corresp, data, right_index=True, left_on='origin_index_u').drop(
             columns=["origin_index_u"]).set_index("origin_index")
 
         if not get_supervision:
             return ret, None, None, None
         else:
@@ -209,18 +211,14 @@
                 df_matrix["f2-score"] = (1 + 2) ** 2 * recall * precision / (2 ** 2 * precision + recall)
 
         return df_matrix
 
     # ==============================================
     #           PLOTS CURVES
     # ==============================================
-    def plot_curves(self):
-        plt.figure(dpi=200, figsize=(7, 5))
-        self.curves.plot(legend=False)
-
     def plot_curves_residual_life(self, **kwargs):
         self.__survival_estimation.plot_residual_life(**kwargs)
         plt.ylabel("Expected residual lifespan")
         plt.xlabel("Time [Y]")
 
     def plot_average_tagged(self, on:str, event_type=None, plot_test_window=False, plot_type="dist"):
         corresp, event, duration, entry = self.__get_align_data(on, get_supervision=True)
@@ -351,37 +349,42 @@
         self.unit = pd.to_timedelta(n_unit, unit=unit).total_seconds()
         self.__check_args()
 
         self.__survival_d = self.survival_function.__deepcopy__()
         self.__survival_d.columns = pd.to_timedelta(self.__survival_d.columns).total_seconds() / self.unit
         self.residual_survival = None
 
-    def plot_residual_life(self, sample=None, mean_behaviour=True):
+    def plot_residual_life(self, sample=None, mean_behaviour=True, unit=pd.to_timedelta(1, "D")):
         if not mean_behaviour:
             if sample is not None:
                 residual_life_ = self.residual_life.sample(sample)
             else:
                 residual_life_ = self.residual_life
             residual_life_.columns = pd.to_timedelta(self.survival_function.columns).total_seconds() / self.unit
             color = plt.get_cmap("magma_r")(residual_life_.iloc[:, 0] / residual_life_.iloc[:, 0].max())
 
             residual_life_.T.plot(legend=False, ax=plt.gca(), color=color, lw=0.15, alpha=1)
             plt.grid()
             bounds = residual_life_.columns.min(), residual_life_.columns.max()
             plt.plot(bounds, bounds[::-1], c="k", alpha=0.5, lw=2, ls="--")
         else:
-            des = self.residual_life.astype("float32").describe([0.05, .25, .5, .75, 0.95])
+            des = (self.residual_life / unit).describe([0.05, .25, .5, .75, 0.95])
             des.columns = pd.to_timedelta(self.survival_function.columns).total_seconds() / self.unit
-
+            des = des.T.dropna().T
             des = des.drop(["count", "mean", "std"])
             for i, d in enumerate(des.index):
                 c = plt.get_cmap("crest")(i / (len(des) - 1))
                 des.loc[d].plot(color=c, ax=plt.gca())
                 if i > 0:
-                    plt.fill_between(des.columns.to_list(), des.iloc[i], des.iloc[i - 1], alpha=0.2, facecolor=c)
+                    plt.fill_between(
+                        des.columns.to_list(),
+                        des.iloc[i],
+                        des.iloc[i - 1],
+                        alpha=0.2,
+                        facecolor=c)
 
             plt.grid()
             plt.legend()
             plt.ylabel("Expected residual lifespan")
             plt.xlabel("Time")
 
     def __check_args(self):
```

### Comparing `survival_data_handler-2024.1.4/survival_data_handler/metric.py` & `survival_data_handler-2024.4.5/survival_data_handler/metric.py`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.1.4/survival_data_handler/plotting.py` & `survival_data_handler-2024.4.5/survival_data_handler/plotting.py`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.1.4/survival_data_handler/utils.py` & `survival_data_handler-2024.4.5/survival_data_handler/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,20 +51,19 @@
 
 
 def compute_derivative(data: pd.DataFrame,
                        unit) -> pd.DataFrame:
     times = data.columns.to_numpy()
     diff = data.T.diff()
     return diff.divide(
-        pd.Series(times, index=times).dt.total_seconds().diff() / unit,
+        pd.Series(times, index=times).diff().dt.total_seconds() / unit,
         axis=0
     ).T
 
 
-
 def _cut(x):
     y = x.copy()
     for i in range(0, y.shape[1] - 1):
         y[:, i] = np.nanmin(y[:, :i + 1], axis=1)
     return y
 
 
@@ -94,41 +93,55 @@
        survival_data = pd.DataFrame(...)  # Provide survival function estimates
        result = residual_life(survival_data)
        ```
 
        References:
        - doi:10.1016/j.jspi.2004.06.012
     """
-    deltas = np.diff(survival_estimate.columns.values)
-
-    # days = deltas.astype('timedelta64[D]').astype(int) / 365.25
-    dt = 1.*np.ones((len(survival_estimate), 1), dtype=precision) * deltas.reshape(
-        1, -1)
-
-    surv_int = survival_estimate.__deepcopy__().astype(float)
+    deltas = - survival_estimate.columns.diff(-1)
+    columns = survival_estimate.columns
+    n = len(survival_estimate)
+
+    dt, t0 = manage_delta(deltas, columns, n, precision)
+
+    survival_int = survival_estimate.__deepcopy__().astype(float)
+    survival_estimate[survival_estimate < 0] = 0
+    survival_estimate[survival_estimate > 1] = 1
 
     s_left = survival_estimate.iloc[:, 1:].values.astype(float)
     s_right = survival_estimate.iloc[:, :-1].values.astype(float)
-    t0 = survival_estimate.columns[0]
-    if "time" in str(dt.dtype):
-        dt = dt / np.timedelta64(1, 's')
-        t0 /= np.timedelta64(1, 's')
-
-    surv_int.iloc[:, :-1] = (s_left + s_right) / 2.
-    surv_int.iloc[:, :-1] *= dt
-    surv_int = surv_int.drop(surv_int.columns[-1], axis=1)
-
-    surv_int = pd.DataFrame(
-        np.cumsum(surv_int[np.sort(surv_int.columns)[::-1]], axis=1),
-        index=surv_int.index,
-        columns=surv_int.columns)
 
-    ret = (surv_int / survival_estimate).astype(precision)
+    survival_int.iloc[:, :-1] = (s_left + s_right) / 2.
+    survival_int.iloc[:, :-1] *= dt[:, :-1]
+    survival_int = survival_int.drop(survival_int.columns[-1], axis=1)
+
+    survival_int = pd.DataFrame(
+        np.cumsum(survival_int[np.sort(survival_int.columns)[::-1]], axis=1),
+        index=survival_int.index,
+        columns=survival_int.columns)
+
+    ret = (survival_int / survival_estimate).astype(precision)
     ret[survival_estimate == 0] = 0
-    return ret - t0
+    ret = ret - t0
+    for c in ret.columns:
+        ret[c] = pd.to_timedelta(ret[c], unit="s")
+    return ret
+
+
+def manage_delta(deltas: np.ndarray, columns, n, precision):
+    if "timedelta" in str(deltas.dtype):
+        deltas_ = pd.to_timedelta(deltas).total_seconds().values
+        dt = 1. * np.ones((n, 1),
+                          dtype=precision) * deltas_.reshape(1, -1)
+        try:
+            t0 = columns[0].total_seconds()
+        except AttributeError:
+            t0 = pd.to_datetime(columns).astype(int)[0] * 1e-9
+    return dt, t0
+
 
 
 class _PoolShift:
     def __init__(self, dates, starting_dates, data):
         self.dates = dates
         self.starting_dates = starting_dates.values
         self.starting_dates_index = starting_dates.index.to_numpy()
```

### Comparing `survival_data_handler-2024.1.4/survival_data_handler.egg-info/PKG-INFO` & `survival_data_handler-2024.4.5/survival_data_handler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survival_data_handler
-Version: 2024.1.4
+Version: 2024.4.5
 Author-email: Vincent Laurent <vlaurent@eurobios.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3
 Requires-Dist: seaborn
 Requires-Dist: numba
 Requires-Dist: scipy
```

### Comparing `survival_data_handler-2024.1.4/test/test_main.py` & `survival_data_handler-2024.4.5/test/test_main.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,22 +85,27 @@
         birth=birth,
         age=age,
         window=(pd.to_datetime("2000"), pd.to_datetime("2100"))
     )
 
     # test plot function
     lifespan.plot_curves_residual_life()
-    lifespan.plot_curves()
     lifespan.add_supervision(event=rossi["arrest"],
                              durations=pd.to_timedelta(rossi["week"] * 7, unit="D"))
 
     assert isinstance(lifespan.survival_function, pd.DataFrame)
     assert isinstance(lifespan.residual_survival(pd.to_datetime("2022")), pd.DataFrame)
     assert isinstance(lifespan.percentile_life(0.1), pd.DataFrame)
     assert isinstance(lifespan.residual_expected_life, pd.DataFrame)
+    assert isinstance(lifespan.density_function, pd.DataFrame)
+    assert isinstance(lifespan.cumulative_hazard_function, pd.DataFrame)
+    assert isinstance(lifespan.hazard_function, pd.DataFrame)
+    assert isinstance(lifespan.lifetime_distribution_function, pd.DataFrame)
+    assert isinstance(lifespan.residual_life, pd.DataFrame)
+
     t = lifespan.compute_times(p=0.5)
     rossi["times"] = t
 
 
 def test_supervision(data):
     from survival_data_handler import test_is_survival_curves
     rossi, curves = data
```

