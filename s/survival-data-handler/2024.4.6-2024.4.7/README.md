# Comparing `tmp/survival_data_handler-2024.4.6.tar.gz` & `tmp/survival_data_handler-2024.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survival_data_handler-2024.4.6.tar", last modified: Mon Apr 29 14:14:21 2024, max compression
+gzip compressed data, was "survival_data_handler-2024.4.7.tar", last modified: Mon Apr 29 16:25:13 2024, max compression
```

## Comparing `survival_data_handler-2024.4.6.tar` & `survival_data_handler-2024.4.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:14:21.049376 survival_data_handler-2024.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-29 14:14:15.000000 survival_data_handler-2024.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-29 14:14:21.049376 survival_data_handler-2024.4.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2108 2024-04-29 14:14:15.000000 survival_data_handler-2024.4.6/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-29 14:14:15.000000 survival_data_handler-2024.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 14:14:15.000000 survival_data_handler-2024.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:14:21.049376 survival_data_handler-2024.4.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:14:21.049376 survival_data_handler-2024.4.6/survival_data_handler/
--rwxr-xr-x   0 runner    (1001) docker     (127)      762 2024-04-29 14:14:15.000000 survival_data_handler-2024.4.6/survival_data_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-29 14:14:15.000000 survival_data_handler-2024.4.6/survival_data_handler/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16908 2024-04-29 14:14:15.000000 survival_data_handler-2024.4.6/survival_data_handler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-29 14:14:15.000000 survival_data_handler-2024.4.6/survival_data_handler/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-29 14:14:15.000000 survival_data_handler-2024.4.6/survival_data_handler/plotting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6365 2024-04-29 14:14:15.000000 survival_data_handler-2024.4.6/survival_data_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:14:21.049376 survival_data_handler-2024.4.6/survival_data_handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-29 14:14:21.000000 survival_data_handler-2024.4.6/survival_data_handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-29 14:14:21.000000 survival_data_handler-2024.4.6/survival_data_handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:14:21.000000 survival_data_handler-2024.4.6/survival_data_handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-29 14:14:21.000000 survival_data_handler-2024.4.6/survival_data_handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 14:14:21.000000 survival_data_handler-2024.4.6/survival_data_handler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:14:21.049376 survival_data_handler-2024.4.6/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5805 2024-04-29 14:14:15.000000 survival_data_handler-2024.4.6/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:25:13.116891 survival_data_handler-2024.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-29 16:25:13.116891 survival_data_handler-2024.4.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2108 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      364 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:25:13.116891 survival_data_handler-2024.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:25:13.116891 survival_data_handler-2024.4.7/survival_data_handler/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      762 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/survival_data_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/survival_data_handler/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15904 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/survival_data_handler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/survival_data_handler/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/survival_data_handler/plotting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6364 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/survival_data_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:25:13.116891 survival_data_handler-2024.4.7/survival_data_handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-29 16:25:13.000000 survival_data_handler-2024.4.7/survival_data_handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-29 16:25:13.000000 survival_data_handler-2024.4.7/survival_data_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:25:13.000000 survival_data_handler-2024.4.7/survival_data_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-29 16:25:13.000000 survival_data_handler-2024.4.7/survival_data_handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 16:25:13.000000 survival_data_handler-2024.4.7/survival_data_handler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:25:13.116891 survival_data_handler-2024.4.7/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6905 2024-04-29 16:25:09.000000 survival_data_handler-2024.4.7/test/test_main.py
```

### Comparing `survival_data_handler-2024.4.6/LICENSE` & `survival_data_handler-2024.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.4.6/PKG-INFO` & `survival_data_handler-2024.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survival_data_handler
-Version: 2024.4.6
+Version: 2024.4.7
 Author-email: Vincent Laurent <vlaurent@eurobios.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3
 Requires-Dist: seaborn
 Requires-Dist: numba
 Requires-Dist: scipy
```

### Comparing `survival_data_handler-2024.4.6/README.md` & `survival_data_handler-2024.4.7/README.md`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.4.6/survival_data_handler/__init__.py` & `survival_data_handler-2024.4.7/survival_data_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.4.6/survival_data_handler/base.py` & `survival_data_handler-2024.4.7/survival_data_handler/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -101,15 +101,16 @@
 
     @property
     def interpolation(self) -> dict:
         if not hasattr(self, "__interpolation"):
             self.__interpolator()
         return self.__interpolation
 
-    def __other(self, other):
+    @staticmethod
+    def __other(other):
         if hasattr(other, "values"):
             return other.values
         else:
             return other
 
 
 class TimeCurveInterpolation(TimeCurve):
@@ -117,29 +118,43 @@
     def __init__(
             self,
             interpolation: dict,
             birth, index: pd.Series,
             window: tuple,
             period):
         self.__interpolation = interpolation
-        self.__birth = birth
-        self.__index = index
-        self.__index.name = 'origin_index'
+
+        self.__matching = pd.DataFrame()
+        self.__matching["index"] = index
+        self.__matching["birth"] = birth
+        self.__matching.index = index.index
+        self.__matching.index.name = 'origin_index'
+
+        self.__reduced_matching = self.__matching.drop_duplicates(
+            subset=["birth", "index"]
+        )
         self.__period = period
         self.__window = window
 
     @property
     def interpolation(self) -> pd.Series:
         return pd.Series(self.__interpolation, name="interpolation")
 
     def __shift(self) -> TimeCurveData:
-        data = pd.merge(self.__index.reset_index(), self.interpolation, right_index=True, left_on='index')
+
+        data = pd.merge(
+            self.__reduced_matching["index"].reset_index(),
+            self.interpolation,
+            right_index=True,
+            left_on='index')
+
         data = data.set_index("origin_index").drop("index", axis=1)
         ret = shift_from_interp(
-            data=data, starting_dates=self.__birth,
+            data=data,
+            starting_dates=self.__reduced_matching["birth"],
             period=self.__period,
             date_initial=self.__window[0],
             date_final=self.__window[1],
             dtypes="float")
         self.__curve = TimeCurveData(ret)
         return self.__curve
 
@@ -148,13 +163,15 @@
         if not hasattr(self, "__curve"):
             self.__shift()
         return self.__curve
 
     @property
     def curve(self) -> TimeCurveData:
         ret = pd.merge(
-            self.__index.reset_index(), self.unique_curve,
+            self.__reduced_matching, self.unique_curve,
             right_index=True,
-            left_index=True).drop(
-            columns=["index"]).set_index("origin_index")
-
+            left_index=True)
+        m = self.__matching
+        ret = pd.merge(m, ret, on=["birth", "index"], how="left")
+        ret.index = m.index
+        ret = ret[self.unique_curve.columns]
         return TimeCurveData(ret)
```

### Comparing `survival_data_handler-2024.4.6/survival_data_handler/main.py` & `survival_data_handler-2024.4.7/survival_data_handler/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,23 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import typing
-
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from sklearn import metrics
 
 from survival_data_handler import plotting
 from survival_data_handler.base import TimeCurveData, SurvivalCurves, TimeCurveInterpolation
-from survival_data_handler.utils import process_survival_function, shift_from_interp
+from survival_data_handler.utils import process_survival_function
 
 # ======================================================================================================================
 # AESTHETICS
 cmap = sns.color_palette('rainbow', as_cmap=True)
 event_censored_color = cmap(0.1)
 event_observed_color = cmap(0.95)
 
@@ -38,32 +36,39 @@
         self.df_idx = pd.DataFrame(dict(age=age, birth=birth, index=index))
 
         self.df_idx.index.name = self.__index
         self.index = index
         self.age = age
         self.window = window
         self.__p = default_precision
-
-        self.__check_args()
-
         self.__survival_estimation = SurvivalEstimation(self.curves, unit='D', n_unit=365.25)
 
-        self._df_idx_unique = self.df_idx.drop_duplicates(subset=["index", "birth"])
-        self.starting_dates = self._df_idx_unique["birth"]
-        c = ["birth", "index"]
+        self.__tci = TimeCurveInterpolation(
+            self.__survival_estimation.survival_function.interpolation,
+            birth,
+            index,
+            window,
+            pd.to_timedelta(30, "D")
+        )
 
-        self._corresp = pd.merge(self._df_idx_unique[c].reset_index(), self.df_idx[c].reset_index(),
-                                 on=["birth", "index"], suffixes=("_u", ""))
+        self.__check_args()
 
-        self._corresp = self._corresp.drop(columns=c)
+        # self._df_idx_unique = self.df_idx.drop_duplicates(subset=["index", "birth"])
+        # self.starting_dates = self._df_idx_unique["birth"]
+        # c = ["birth", "index"]
+
+        # self._corresp = pd.merge(self._df_idx_unique[c].reset_index(), self.df_idx[c].reset_index(),
+        #                          on=["birth", "index"], suffixes=("_u", ""))
+        #
+        # self._corresp = self._corresp.drop(columns=c)
         self.confusion_matrix_threshold = np.nan
         self.__computed = []
         self.__supervised = False
         self.__interpolator = {}
-        super().__init__(self.survival_function)
+        super().__init__(self.__tci.curve)
 
     def __check_args(self):
 
         if hasattr(self.curves.columns, "dt"):
             ValueError("curves index must have dt property")
 
     @property
@@ -85,73 +90,45 @@
         if not get_supervision:
             return ret, None, None, None
         else:
             index = [i for i in ret.index if i in self.event.index]
             entry = self.entry if self.entry is None else self.entry.loc[index]
             return ret.loc[index], self.event.loc[index], self.durations.loc[index], entry
 
-    def _decompose_unique(self, data, get_supervision=False):
-        ret = pd.merge(self._corresp, data, right_index=True, left_on='origin_index_u').drop(
-            columns=["origin_index_u"]).set_index("origin_index")
-
-        if not get_supervision:
-            return ret, None, None, None
-        else:
-            index = [i for i in ret.index if i in self.event.index]
-            entry = self.entry if self.entry is None else self.entry.loc[index]
-            return ret.loc[index], self.event.loc[index], self.durations.loc[index], entry
-
-    # ==============================================
-    #           PROPERTIES
-    # ==============================================
-    @property
-    def survival_function(self) -> pd.DataFrame:
-        if "survival_function" not in self.__interpolator.keys():
-            self.__interpolator["survival_function"] = self.__compute_curve("survival_function")
-        return self.__interpolator["survival_function"].curve
+    # def _decompose_unique(self, data, get_supervision=False):
+    #     ret = pd.merge(self._corresp, data, right_index=True, left_on='origin_index_u').drop(
+    #         columns=["origin_index_u"]).set_index("origin_index")
+    #
+    #     if not get_supervision:
+    #         return ret, None, None, None
+    #     else:
+    #         index = [i for i in ret.index if i in self.event.index]
+    #         entry = self.entry if self.entry is None else self.entry.loc[index]
+    #         return ret.loc[index], self.event.loc[index], self.durations.loc[index], entry
 
     @property
     def residual_expected_life(self) -> pd.DataFrame:
-        if "residual_life" not in self.__interpolator.keys():
-            self.__interpolator["residual_life"] = self.__compute_curve("residual_life")
-        return self.__interpolator["residual_life"].curve
+        return self.residual_life
 
     # ==============================================
     #           ENRICH REPRESENTATION
     # ==============================================
 
-    def __compute_curve(self, attribute):
-        self.index.index.name = None
-        tci = TimeCurveInterpolation(
-            self.__survival_estimation.__getattribute__(attribute).interpolation,
-            self._df_idx_unique["birth"],
-            self.index,
-            self.window,
-            pd.to_timedelta(30, "D")
-        )
-        return tci
-
     def residual_survival(self, t0) -> pd.DataFrame:
 
         t0 = max(t0, self.survival_function.columns[0])
         s0 = get(self.survival_function, t0).astype("float16").values
         df = self.survival_function.divide(s0, axis=0).copy()
         df = df[[c for c in df.columns if c > t0]]
         return df
 
     def compute_times(self, p=0.95, on="survival_function"):
-
         cond_low = (self.__getattribute__(on) > p).sum(axis=1)
         dates = self.__getattribute__(on).columns.to_numpy()
-        df_time = self._df_idx_unique.__deepcopy__()
-        df_time.loc[cond_low.index, "time"] = dates[
-            np.where(cond_low.values >= len(dates), len(dates) - 1, cond_low.values)]
-        # remove past positive sample
-        df_time, _, _, _ = self._decompose_unique(df_time)
-        return df_time["time"]
+        return pd.Series(dates[cond_low])
 
     def remove_the_dead(self, data: pd.DataFrame, error="coerce"):
         try:
             data = data.loc[self.event.index[~self.event.astype(bool)]]
         except KeyError as e:
             print(e)
 
@@ -216,15 +193,15 @@
     #           PLOTS CURVES
     # ==============================================
     def plot_curves_residual_life(self, **kwargs):
         self.__survival_estimation.plot_residual_life(**kwargs)
         plt.ylabel("Expected residual lifespan")
         plt.xlabel("Time [Y]")
 
-    def plot_average_tagged(self, on:str, event_type=None, plot_test_window=False, plot_type="dist"):
+    def plot_average_tagged(self, on: str, event_type=None, plot_test_window=False, plot_type="dist"):
         corresp, event, duration, entry = self.__get_align_data(on, get_supervision=True)
         if event_type == "censored":
             sample = corresp[~event.astype(bool)].astype("float32")
             color = event_censored_color
         elif event_type == "observed":
             sample = corresp[event.astype(bool)].astype("float32")
             color = event_observed_color
@@ -255,15 +232,15 @@
             t0 = duration[event.astype(bool)].min()
             t1 = duration[event.astype(bool)].max()
 
             plt.axvline(t0, lw=1.5, ls="--", color="k")
             plt.axvline(t1, lw=1.5, ls='--', color="k", label="Test window")
         plt.legend()
 
-    def plot_dist_facet_grid(self, on:str, n=4):
+    def plot_dist_facet_grid(self, on: str, n=4):
         bins = np.linspace(0, 1, 50)
         data, event, duration, entry = self.__get_align_data(on, get_supervision=True)
         s = data.shape[1]
         dates = data.columns.to_numpy()[np.array([(s * i) // n for i in range(1, n)])]
 
         df = data[dates].unstack().reset_index()
         data["event"] = event
@@ -272,15 +249,15 @@
         df["dates"] = df["dates"].dt.year
 
         g = sns.FacetGrid(df, row="dates", hue="event", aspect=5, height=2, palette="RdBu_r")
         g.map(sns.histplot, "survival", fill=False, alpha=1, linewidth=2, bins=bins, element="step",  # cumulative=True,
               stat="density", common_norm=False)
         plt.legend()
 
-    def plot_tagged_sample(self, on:str, n_sample=None, n_sample_pos=None, n_sample_neg=None, ):
+    def plot_tagged_sample(self, on: str, n_sample=None, n_sample_pos=None, n_sample_neg=None, ):
 
         assert self.__supervised, "No supervision provided"
         data, event, duration, entry = self.__get_align_data(on, get_supervision=True)
         if n_sample is None and n_sample_neg is None and n_sample_pos is None:
             sample = data
         elif n_sample_pos is None and n_sample_neg is None:
             sample = data.sample(n_sample)
```

### Comparing `survival_data_handler-2024.4.6/survival_data_handler/metric.py` & `survival_data_handler-2024.4.7/survival_data_handler/metric.py`

 * *Files identical despite different names*

### Comparing `survival_data_handler-2024.4.6/survival_data_handler/plotting.py` & `survival_data_handler-2024.4.7/survival_data_handler/plotting.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,45 +41,14 @@
         plot.plot(outdated.loc[pos_index].T, c=event_observed_color,
                   **plot_args)
     plot_args = dict(lw=1, alpha=0.9)
     plot.plot(temp_curves.loc[pos_index].T, c=event_observed_color, **plot_args)
     plot.plot(temp_curves.loc[neg_index].T, c=event_censored_color, **plot_args)
 
 
-def _prepare_data(duration,
-                  event,
-                  entry,
-                  temporal_score: pd.DataFrame
-                  ):
-    label = event
-    time_event = duration
-    temp_curves = temporal_score.astype("float32")
-    temp_curves.index = range(len(temp_curves))
-    dates = temp_curves.columns.to_list()
-    pos_index = temp_curves.index[label.astype(bool)]
-    # check consistency
-    if time_event is not None:
-        col_id = np.searchsorted(temp_curves.columns, time_event) - 1
-
-        outdated = pd.DataFrame(np.nan, index=temp_curves.index,
-                                columns=temp_curves.columns)
-        for c in np.unique(col_id):
-            ind = col_id == c
-            data = temp_curves[ind]
-            outdated.loc[ind, dates[c:]] = data[dates[c:]]
-            temp_curves.loc[ind, dates[c + 1:]] = np.nan
-        temp_curves["observed"] = True
-        outdated["observed"] = False
-        data = pd.concat((temp_curves, outdated), axis=0)
-
-        data["observed event"] = False
-        data.loc[pos_index, "observed event"] = True
-        return data
-
-
 def auc_vs_score_plotly(
         temporal_scores: pd.DataFrame,
         event_observed: pd.Series,
         censoring_time: pd.Series,
         entry_time: pd.Series,
         temporal_metric: pd.Series,
         event_observed_color=default_event_observed_color_2,
```

### Comparing `survival_data_handler-2024.4.6/survival_data_handler/utils.py` & `survival_data_handler-2024.4.7/survival_data_handler/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,14 @@
         try:
             t0 = columns[0].total_seconds()
         except AttributeError:
             t0 = pd.to_datetime(columns).astype(int)[0] * 1e-9
     return dt, t0
 
 
-
 class _PoolShift:
     def __init__(self, dates, starting_dates, data):
         self.dates = dates
         self.starting_dates = starting_dates.values
         self.starting_dates_index = starting_dates.index.to_numpy()
         self.data = data.values
         self.data_index = data.index.to_numpy()
```

### Comparing `survival_data_handler-2024.4.6/survival_data_handler.egg-info/PKG-INFO` & `survival_data_handler-2024.4.7/survival_data_handler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survival_data_handler
-Version: 2024.4.6
+Version: 2024.4.7
 Author-email: Vincent Laurent <vlaurent@eurobios.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3
 Requires-Dist: seaborn
 Requires-Dist: numba
 Requires-Dist: scipy
```

### Comparing `survival_data_handler-2024.4.6/test/test_main.py` & `survival_data_handler-2024.4.7/test/test_main.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import pandas as pd
+import numpy as np
 import pytest
 from lifelines import CoxPHFitter
 from lifelines.datasets import load_rossi
 
 from survival_data_handler.main import SurvivalEstimation, Lifespan, TimeCurveData
 from survival_data_handler.utils import smooth, process_survival_function, \
     compute_derivative
@@ -74,15 +75,19 @@
 
 
 def test_lifespan(data):
     rossi, curves = data
 
     age = pd.to_timedelta(rossi["age"] * 365.25, unit="D")
     birth = pd.to_datetime('2000')
-    rossi["index"] = rossi.index
+    curves = curves.iloc[:2]
+    curves.index = ["a", "b"]
+
+    rossi["index"] = np.random.choice(curves.index, replace=True, size=len(rossi))
+
     lifespan = Lifespan(
         curves,
         index=rossi["index"],
         birth=birth,
         age=age,
         window=(pd.to_datetime("2000"), pd.to_datetime("2100"))
     )
@@ -145,19 +150,47 @@
 
 
 def test_interpolation_curves(data):
     rossi, curves = data
     rossi["duration"] = pd.to_timedelta(rossi["week"]*7, unit="D")
     rossi["birth"] = pd.to_datetime('2000')
     rossi["index"] = rossi.index
+    curves = curves.iloc[:2]
+    curves.index = ["a", "b"]
+
+    rossi["index"] = np.random.choice(curves.index, replace=True, size=len(rossi))
+    tc = TimeCurveData(curves)
+    tc_prime = tc.interpolation
+
+    ti = TimeCurveInterpolation(
+        interpolation=tc_prime,
+        index=rossi["index"],
+        birth=rossi["birth"],
+        period=pd.to_timedelta(30, "D"),
+        window=(pd.to_datetime("2000"), pd.to_datetime("2001")))
+
+    assert isinstance(ti.unique_curve, TimeCurveData)
+    assert isinstance(ti.curve, TimeCurveData)
+    assert len(ti.unique_curve) == 2
+    assert len(ti.curve) == len(rossi)
+
+    rossi, curves = data
+    rossi["duration"] = pd.to_timedelta(rossi["week"]*7, unit="D")
+    rossi["birth"] = pd.to_datetime('2000')
+    rossi["index"] = rossi.index
 
+    rossi["index"] = np.random.choice(curves.index, replace=True, size=len(rossi))
     tc = TimeCurveData(curves)
     tc_prime = tc.interpolation
 
     ti = TimeCurveInterpolation(
-        tc_prime,
+        interpolation=tc_prime,
         index=rossi["index"],
         birth=rossi["birth"],
         period=pd.to_timedelta(30, "D"),
         window=(pd.to_datetime("2000"), pd.to_datetime("2001")))
+
     assert isinstance(ti.unique_curve, TimeCurveData)
     assert isinstance(ti.curve, TimeCurveData)
+    assert len(ti.unique_curve) <= len(rossi)
+    assert len(ti.curve) == len(rossi)
+
```

